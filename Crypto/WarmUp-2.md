### By: [Sahil Bugade](http://snip3r.me)

## Problem Statement:
![image](https://user-images.githubusercontent.com/116542156/197476020-fb3f226c-ef75-42f1-8bea-8ff35e481ce5.png)

## Solution:

Given Ciphertext: fzvxw{hqtegmfr_lw_msf_scrslg_kvwlhyk_fpr_kxg?}
Hint: The Key to success is `Determination`.

So with the first look at the ciphertext we couldn't guess which encryption algorithm is used in it. So we simply use the open-source tool [cipher-identifier] (https://www.boxentriq.com/code-breaking/cipher-identifier) to find the type of algorithm.

![image](https://user-images.githubusercontent.com/116542156/197477291-4c0fc6ca-a9cb-4394-b20b-36e1388c6ddd.png)

So after analyzing the text it shows us that the encryption algorithm used is Vigenere Autokey Cipher. So we proceed to use the decryptor for the mentioned algorithm.

![image](https://user-images.githubusercontent.com/116542156/197477384-cdd95fa6-d2cc-4534-854f-f7811b628304.png)

As we can see there is an option asking us for the key and also we can see the problem statement mentioning a hint saying the key to success is “Determination”. So that’s it, just some copypasta and we are here with the flag: cvctf{vigenere_is_too_guessy_without_the_key?}

![image](https://user-images.githubusercontent.com/116542156/197477461-835e707e-ef0e-4a3c-9bfd-9526028c89f7.png)

### Flag: cvctf{vigenere_is_too_guessy_without_the_key?}

We even tried to auto decode the message but it was a lot confusing and time consuming at the same time so we have to utilize all the hints given according to the encryption/decryption format.
