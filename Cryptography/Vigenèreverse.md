# Vigenèreverse (Cryptography) - 69
> I love reversing things and using the Vigenère cipher, but I despise plaintext keys. Can you help me encrypt the key before you decrypt the ciphertext flag?
> 

`Flag: sunctf25{f0rW4Rd_bUt_0ppO5iTe}`

# Solution

### 1. Examining the File Contents
We are provided with a text file, `virev.txt` which contains the content to be decrypted. The file’s content consists of a cipertext and a plaintext key required to decode the cipher.

<img width="845" height="667" alt="image" src="https://github.com/user-attachments/assets/2bab7b82-92f9-4632-84e3-15a2692fa045" />

### 2. Examining the Challenge's Description
Firstly, the challenge's description is analyzed to search for potential information and hints. 

According to the challenge's description, we are required to encrypt the key before decrypting the ciphertext flag. We are also provided with additional information that the creator despises plaintext keys and loves to reverse things using the Vigenere cipher. Hence, we can assume that we are required to reverse the plaintext key and utilize it as the key to encrypt the plaintext key with Vigenere cipher. The encrypted key is then utilized to decode the cipertext. 

<img width="514" height="478" alt="image" src="https://github.com/user-attachments/assets/5960ea67-6cb6-4e0b-b6e2-6d932dc50d62" />

### 3. Reversing the Key
With the required information, we start off by reversing the given key with the help of Cyberchef's Reverse function, which will return us with an output of `emesrevertnod`

<img width="1936" height="930" alt="image" src="https://github.com/user-attachments/assets/116c5a2d-109b-4dcf-af08-cad715204627" />

### 4. Encrypting the Key
Moving on, we can use the reversed key to encrypt the plaintext key using Vigenère cipher to return us the encrypted key with the help of Cyberchef's Vigenère Encode function. This will return us the encrypted key, `harliiqiilrah`

<img width="1936" height="930" alt="image" src="https://github.com/user-attachments/assets/6aa97d4e-62c0-4701-9bac-49d25d81e579" />

### 5. Obtaining the Flag
By using the newly obtained encrypted key, `harliiqiilrah`, we can now decrypt the ciphertext using Cyberchef's Vigenère Decode function, which will reveal the flag, `sunctf25{f0rW4Rd_bUt_0ppO5iTe}`.

<img width="1936" height="930" alt="image" src="https://github.com/user-attachments/assets/69439191-0e4c-4594-9322-3b4dc68c4731" />




