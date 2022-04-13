<h1 align="center"> CryptoJS - PBKDF2 - SHA512 - AES </h1>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)


## 👇 1. PBKDF2

PBKDF2 is a password-based key derivation function. In many applications of cryptography, user security is ultimately dependent on a password,
    and because a password usually can't be used directly as a cryptographic key, some processing is required.
    A salt provides a large set of keys for any given password, and an iteration count increases the cost of producing keys from a password,
    thereby also increasing the difficulty of attack.

## 👇 2. SHA-2

SHA-2 (Secure Hash Algorithm 2) is a set of cryptographic hash functions designed by the United States National Security Agency (NSA) 
      and first published in 2001.[3][4] They are built using the Merkle–Damgård construction, from a one-way compression function itself built using the Davies–Meyer 
      structure from a specialized block cipher

## 👇 3. AES
The Advanced Encryption Standard (AES), also known by its original name Rijndael 
      is a specification for the encryption of electronic data established by
      the U.S. National Institute of Standards and Technology (NIST) in 2001.[4]

# 🚀 Encrypt

Using PBKDF2 to generate key derivation:

```
let encryptedKey = CryptoJS.PBKDF2(password, salt, { hasher: CryptoJS.algo.SHA512, keySize, iterations });
```

Using AES with custom IV to encode

```
let encryptedMessage = CryptoJS.AES.encrypt(planText, encryptedKey, { iv: iv });
```

# 🚀 Decrypt
Using PBKDF2 to generate key derivation:

```
let decryptedKey = CryptoJS.PBKDF2(password, salt, { hasher: CryptoJS.algo.SHA512, keySize, iterations });
```

Using AES with custom IV to decode

```
let decryptedMessage = CryptoJS.AES.decrypt(encryptedMessage, decryptedKey, { iv: iv });
```

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png)

## ✨ Contributing
Please feel free to contact me or make a pull request.

## 👇 Authors
``` Created by $username on $today
Copyright (c) $today.year . All rights reserved.
Last modified $file.lastModified
```
<p>
    <a href="https://nphau.medium.com/" target="_blank">
    <img src="https://avatars2.githubusercontent.com/u/13111806?s=400&u=f09b6160dbbe2b7eeae0aeb0ab4efac0caad57d7&v=4" width="96" height="96">
    </a>
</p>
