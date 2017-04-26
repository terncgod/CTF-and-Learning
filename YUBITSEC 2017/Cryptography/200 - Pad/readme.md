- We was given this [Encrypter](https://github.com/kuqadk3/CTF-and-Learning/blob/master/YUBITSEC%202017/Cryptography/200%20-%20Pad/advanced_enc.py)

- And was given this [Encrypted message](https://github.com/kuqadk3/CTF-and-Learning/blob/master/YUBITSEC%202017/Cryptography/200%20-%20Pad/encrypted_2)

- To decrypt it,we use this formula :



int formula = int(encrypted_message[i]) - int(start_char) + n x modular + 2 x int(start_char) - int(key[i])



With i = 0 and n = 1, we have :

int formula = 36 - 32 + 1 x 95 + 2 x 32 - 74 = 89 -> "Y"

- Sample decoder coded in C++ : [Decoder](https://github.com/kuqadk3/CTF-and-Learning/blob/master/YUBITSEC%202017/Cryptography/200%20-%20Pad/decoder.cpp)

- After decrypt it all, we got flag : YUBITSEC{going_through}