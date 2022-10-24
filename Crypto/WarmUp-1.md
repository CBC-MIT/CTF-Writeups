### By: [Sahil Bugade](http://snip3r.me)

## Problem Statement:

![image](https://user-images.githubusercontent.com/116542156/197474571-3771fd8a-ff3c-418e-a276-84f84aaf8ed7.png)

## Solution:
Given cipher text: cGlwZ3N7cG5yZm5lXzY0X3Nnan0=

Now after solving a bit of crypto CTFs we were easily able to guess that the given cipher text was encoded in base64. So firstly we decoded it from base64.

![image](https://user-images.githubusercontent.com/116542156/197474910-854c8538-a5f5-421f-a342-e1fcf88ef02f.png)

As you can see the decode text is “pipgs{pnrfne_64_sgj}” which can be identified as a format that a flag would be written in but isn’t the actual flag as the competition had its flag format “cvctf{}”.

So hereby, I saw that the output we got had (PiPgs) repeated “P” and the flag format (CvCtf) had “C” repeated. So I calculated how far is the alphabet “C” from “P” and came out to be 13 letters ahead.

So I calculated manually each and every alphabet 13 ahead of the given decoded form and came out with the flag cvctf{caesar_64_ftw}.

Later I came to know that such type of encryption is called ROT-13 encryption and could be found on the site: [ROT-13 Decoder](https://www.dcode.fr/rot-13-cipher)

![image](https://user-images.githubusercontent.com/116542156/197475221-ace9ee60-783d-411f-9e6d-e94dbeba9b60.png)

### Flag: cvctf{caesar_64_ftw}

It was our first international CTF, so overall we enjoyed it and to mention teamwork is always a key to success!
