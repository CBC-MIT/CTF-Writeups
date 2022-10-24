### By: [Ananya Sharma](https://www.linkedin.com/in/ananya-sharma-2699a2250/)

## Problem Statement:

![image](https://user-images.githubusercontent.com/116542156/197478444-2fcb47af-26cc-4b55-90a7-0e588117d4a6.png)

## Solution:

In this CTF, we were given a question where we had to find flag from a given unknown encrypted text. In this CTF the unknown encrypted text was given in text file. The question was given in such a way shown in the image above.

After downloading the text file. We could see that there were random letters arranged as shown below in the image.

![image](https://user-images.githubusercontent.com/116542156/197478848-fa4ae68b-d37b-4b02-9c3b-e063e1838ff9.png)

Then our fist task was to find out what kind Cipher or what encryption way is used to encrypt it. So, we used [Cipher identifier](https://www.boxentriq.com/code-breaking/cipher-identifier) tool available on internet.

After that, we pasted texted the text and used the tool and the tool indicated that the given text is encrypted in Base64.

![image](https://user-images.githubusercontent.com/116542156/197479192-020b571f-63c6-4274-8c65-d458761ca366.png)

Then we used [Base64 decode](https://www.base64decode.org/) tool available on internet to decode this text.

After putting the text we got Hex values.

![image](https://user-images.githubusercontent.com/116542156/197479376-54797ff4-3d14-419e-9f25-f285826d1007.png)

As the output directly shows that the we got Hex values. Then we used tool [Cyber Chef tool](https://gchq.github.io/CyberChef/) available on internet to decode these Hex values.

For using the tool we had to choose “From Hex” operation to decode the hex value.

![image](https://user-images.githubusercontent.com/116542156/197479669-bc1e3d14-e392-456f-b0d4-5ac23706f86a.png)

From the output, we were getting some random texts so we tried to use magic function provided by the tool to automatically decode the text. So, then we used it again we got another series of random text.

![image](https://user-images.githubusercontent.com/116542156/197479853-13f63167-2b74-43c2-b04b-e7a5a3ad93b7.png)

After that again we used magic tool. After using magic tool, we could see random emojis as output.

![image](https://user-images.githubusercontent.com/116542156/197479974-d09501ce-9830-48fd-ad2e-9172f49e1d7e.png)

After getting this output, I was completely confused as I had never seen such output before. I thought I made any mistake so I performed it multiple times but still I was getting same output. Then I starting searching on internet about such output. After a long research got to know that there is another type of cipher known as Emoji cipher. I found it really different from other ciphers that exist. So, I started looking for tools to decode emoji ciphers. On internet I found a tool called [Cryptoji](https://cryptoji.com/) which helps in encrypting as well as decrypting emoji ciphers.

Then I copied the emoji from cyber chef tool and pasted in cryptoji tool to decode this and finally I got what I was looking for, The flag. After getting flag there was a special kink of satisfaction.

![image](https://user-images.githubusercontent.com/116542156/197480396-c62ca15b-58ad-436b-a428-90dc5fc7393a.png)

### Flag- cvctf{3m0j1_c4n_L34K_7h1ng5}

So this was my experience of solving this CTF question.

Note- Always consider all the possibilities.
