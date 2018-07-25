---
ID: 169
post_title: Cryptography Activity
author: admin
post_excerpt: ""
layout: post
permalink: >
  http://localhost:8000/cryptography-activity/
published: true
post_date: 2018-07-25 10:21:47
---
This activity focuses on exploring some of the oldest cryptographic methods which can be used to secure information. We also look at the vulnerabilities in their designs.   [objective aim="understand the purpose of cryptography."] [skill]Use the Caesar and <span style="font-weight: 400;">Vigenère </span> Ciphers[/skill] [skill]Understand weaknesses of basic cryptographic techniques[/skill] [/objective]   
## <span style="font-weight: 400;">Caesar Cipher</span>

<span style="font-weight: 400;">One of the oldest forms of the encryption is the Caesar cipher. Named after Julius Caesar, the first to report using it, it is very simple. Each character shifts a fixed number of places in the alphabet, wrapping around to the beginning if necessary.</span>   <span style="font-weight: 400;">Caesar cipher is a class of cipher called substitution cipher. A character represents the key to the cipher. For example, consider the key “</span>**c**<span style="font-weight: 400;">”, “</span>**c**<span style="font-weight: 400;">” is the 3rd letter in the alphabet so all characters get shifted to the left 3 places. The substitution for “</span>**c**<span style="font-weight: 400;">” as the key will be:</span>   
<table>
  <tbody>
    <tr>
      <td colspan="26">
        <p style="text-align: center;">
          <span style="color: #3366ff;"><b>Plain character</b></span>
        </p>
      </td>
    </tr>
    
    <tr>
      <td>
        <span style="color: #3366ff;"><b>A</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>B</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>C</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>D</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>E</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>F</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>G</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>H</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>I</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>J</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>K</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>L</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>M</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>N</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>O</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>P</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>Q</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>R</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>S</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>T</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>U</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>V</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>W</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>X</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>Y</b></span>
      </td>
      
      <td>
        <span style="color: #3366ff;"><b>Z</b></span>
      </td>
    </tr>
    
    <tr>
      <td>
        <span style="color: #ff0000;"><b>C</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>D</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>E</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>F</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>G</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>H</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>I</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>J</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>K</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>L</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>M</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>N</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>O</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>P</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>Q</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>R</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>S</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>T</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>U</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>V</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>W</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>X</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>Y</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>Z</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>A</b></span>
      </td>
      
      <td>
        <span style="color: #ff0000;"><b>B</b></span>
      </td>
    </tr>
    
    <tr>
      <td colspan="26">
        <p style="text-align: center;">
          <span style="color: #ff0000;"><b>Cipher character</b></span>
        </p>
      </td>
    </tr>
  </tbody>
</table>   

<span style="font-weight: 400;">The ciphertext of the plaintext message “University of Leeds” using “c” as the key will be:</span>   <h6 style="text-align: center;">
  <b>WPKXG TUKVA QHJGG FU</b>
</h6>   

<span style="font-weight: 400;">Spaces are ignored and then the cipher characters are grouped into groups of 5 to obscure the length of individual words.</span>     [step number="1" title="Your Turn: Caesar Encryption"] **You are now going to have a go at encrypting some text using a Caesar cipher.** [substep]<span style="font-weight: 400;">In pairs or small groups use the cipher wheels to encrypt your name using a Caesar cipher, you can choose the key as any character.</span>[/substep] **Encrypting text is a dull task which is easily automated by a computer. You are now going to use a script to do the same task.** [substep]<span style="font-weight: 400;">Enter your names into a file called names.txt (using gedit) and use the encryption script to encrypt your name using the same key as you did in part (1). Check the result and see if you encrypted your name correctly.</span>[/substep]   <span style="font-weight: 400;">[info]To encrypt using the script run the following command[/info]</span>   [code lang="python"]./encrypt.py -f names.txt -key <INSERT YOUR KEY HERE[/code] [/step]   <span style="font-weight: 400;">[step number="2" title="Your Turn: Caesar Decryption"]</span>   <span style="font-weight: 400;">[substep]Enter your encrypted name into a file called ciphernames.txt (using gedit) and use the decryption script to decrypt your name. Check the result and see if your name is deciphered.[/substep]</span>   <span style="font-weight: 400;">[info]To decrypt using the script run the following command[/info]</span> <span style="font-weight: 400;">./decrypt.py -f ciphernames.txt -key <INSERT YOUR KEY HERE></span>   [/step]   
## <span style="font-weight: 400;">Caesar Cipher Vulnerability</span>

<span style="font-weight: 400;">Caesar cipher is a very simple cryptographic system, which is not used in practice were security is important this is because Caesar cipher is vulnerable to a simple attack. There are only 26 possible key which can be used to encrypt/decrypt plaintext, to find the key we need only try each key and establish whether the result produced looks like English. To establish if it looks like English we can use a technique called letter frequency analysis. This technique relies on the fact that some letters appear more often in English text than other. The  7 most common letters are:</span>   <h6 style="text-align: center;">
  <b>E T A O I N S</b>
</h6>   

**This attack is known as letter frequency analysis.**         [step number="3" title="Your Turn: Caesar Cracking"] **You are now going to have a go at cracking some codes.** [substep]<span style="font-weight: 400;">Using the decrypt script try and discover the key for the file ciphertext. If the key is correct the output will be in plain English. You will have to try all possible keys.</span>[/substep] [substep]<span style="font-weight: 400;">Using the character frequency script discover the key for the ciphertext file. Read the output of the script carefully. The key is calculated by setting ‘E’ on the cipher wheel to be the most commonly occurring letter from the frequency analysis. If the most common letter does not decipher the text try the next most common letter.</span>[/substep]   [info]<span style="font-weight: 400;">To apply frequency analysis using the script run the following command</span> [/info] <span style="font-weight: 400;">./charfreq.py -f ciphertext</span> [excl]Y<span style="font-weight: 400;">ou may find it easier to read the output of this programme by maximising the window</span>[/excl] [substep]<span style="font-weight: 400;">Use the decrypt script from before to decrypt the ciphertext file using the key you have discovered.</span>[/substep] [/step]   
## <span style="font-weight: 400;">Vigenère Cipher</span>

<span style="font-weight: 400;">Vigenère cipher is a stronger cryptographic system but has some commonalities with the caesar cipher. Vigenère is a polyalphabetic substitution cipher, this means that instead of having a single key it now has a key of variable length.</span>   <span style="font-weight: 400;">The plaintext is encrypted using a key, for example, if we let the key be “SOC”. The first letter of the plaintext is encrypted using the first letter of the key, the second letter of the plaintext is encrypted using the second letter of the key and so on. When we encounter the end of the key we go back to the start of the key and use the first letter again. The encryption used is the caesar cipher. For example, to encrypt “School of Computing” using the key “SOC” we would get</span>   
<table>
  <tbody>
    <tr>
      <td>
        <span style="font-weight: 400;">Plaintext</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">H</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">L</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">F</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">M</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">P</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">U</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">T</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">I</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">N</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">G</span>
      </td>
    </tr>
    
    <tr>
      <td>
        <span style="font-weight: 400;">Key</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">C</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">S</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
    </tr>
    
    <tr>
      <td>
        <span style="font-weight: 400;">Ciphertext</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">K</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">Q</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">J</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">G</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">O</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">N</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">G</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">T</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">E</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">G</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">A</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">R</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">M</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">H</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">K</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">F</span>
      </td>
      
      <td>
        <span style="font-weight: 400;">U</span>
      </td>
    </tr>
  </tbody>
</table>     [step number="4" title="Your Turn: Vigenère Encryption"] 

**You are now going to encrypt some text using Vigenère cipher.** [substep]<span style="font-weight: 400;">Using the key “UOL” encrypt the name of your school/college using the Vigenère table.</span>[/substep] **Remember, encrypting text is a dull task which is easily automated by a computer! Let's use a script to do the same task.** [substep]<span style="font-weight: 400;">Enter the name of your school into a file called school (using gedit) and use the Vigenère</span> <span style="font-weight: 400;">encryption script to encrypt it. Check the result and see if you encrypted it correctly.[/substep]</span> <span style="font-weight: 400;">To encrypt using the script run the following command</span> <span style="font-weight: 400;">./encryptvig.py -f school -key UOL</span> [/step]   
## <span style="font-weight: 400;">Vigenère Cipher vulnerability</span>   

<span style="font-weight: 400;">The vigenère cipher is similar to caesar cipher and as a result suffers from a similar vulnerability, however it is a little bit more complex to find the key because the key is now comprised of many letters. There are no longer 26 possible keys but instead, there are </span><span style="font-weight: 400;">26</span><span style="font-weight: 400;">n</span><span style="font-weight: 400;"> possible keys, where n is the length of the key.  This relatively massive set of possible keys makes it impractical to brute force attack the key. </span>   <span style="font-weight: 400;">If we know that the vigenère cipher has been used then we can use letter frequency analysis again but we have to “guess” the length of the key. Suppose the key has length 3 then we know that the 1st, 4th, 7th…. letters of the ciphertext have been encrypted using the same character of the key and that the 2rd, 5th, 8th…. letters of the ciphertext have been encrypted using the same character of the keys and that the 3rd, 6th, 9th…. letters of the ciphertext have been encrypted using the same character of the key. We can simply use the letter frequency analysis on these letters of the ciphertext to discover the 1st, 2nd and 3rd characters of the key.</span>     [step number="5" title="Your Turn: Vigenère Cracking"] **You are now going to crack a Vigenère cipher.** [substep]<span style="font-weight: 400;">Using the script discover the key used to encrypt the file ciphertext_vig. Read the output of the script carefully to discover the key. The script will output the frequency analysis for a given key length.</span>[/substep] <span style="font-weight: 400;">To discover the key used to encrypt use the following command. </span> <span style="font-weight: 400;">./charfreqvig.py -f ciphertext_vig -l <possible key length></span> <span style="font-weight: 400;">[info]</span>**HINT**<span style="font-weight: 400;">: the length of the key is between 2-8[/info]</span>   [substep]<span style="font-weight: 400;">Using the script decrypt the file ciphertext_vig using the key you discovered previously.</span><span style="font-weight: 400;">[/substep]</span> <span style="font-weight: 400;">To decrypt the vigenère cipher use the following command.</span>   <span style="font-weight: 400;">./decryptvig.py -f ciphertext_vig -key <insert key here></span> [/step]       [finish] 
### <span style="font-weight: 400;">What’s next?</span>

<span style="font-weight: 400;">Neither of the ciphers are particularly “good”, what else exists?</span> <span style="font-weight: 400;">What role do computers play in cryptography?</span> <span style="font-weight: 400;">How does this relate to modern day life?</span> <span style="font-weight: 400;">How does this relate to our degree?</span> [/finish]