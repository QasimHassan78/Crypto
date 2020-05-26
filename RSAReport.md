DM 103347: **RSA Algorithm**

PROJECT MEMBERS

**62357** | **Qasim Hassan**

62553 | Nabeel Anwer

62366 | Zahida Naz

**Project Description**

The RSA algorithm is developed by Ron rivest, Adishamir and Leonard adleman in the year 1977. It is also known as public key encryption algorithm 1. The modern computers utilize RSA for encryption and decryption. It uses two different keys one for encryption process and another for decryption. Anyone with the public key can encrypt the data while decryption is only done by that person who has the private key.

Today it is widely used in email programs, web browsers, virtual private networks and mobile phones 1. RSA introduced when the electronic mails era was expected to soon arise, it focused two vital ideas:

**1. Public-key encryption.** This concept omits the courier need for the delivery of keys to the recipients by secure medium before sending the original message. In this algorithm everyone owns his personal encryption and decryption keys. The keys are designed such that the decipherment key may not be easily cracked from the public encryption key 2.

**2. Digital signatures.** On the receiving side the verification of transmitted message is necessary so that we can assure that this is sent by the actual sender and didn&#39;t just come from anyone. We make it possible by using sender&#39;s decryption key, and finally the signature is verified by anybody, who is using the particular public encryption key. By doing this no signer can deny that he doesn&#39;t signed the message 2.

We can use RSA not only in electronic mail but also for other electronic transactions as well, for example fund transfer. This algorithm is not easily cracked by invaders because of difficulty in factoring large numbers n= pq. Here p and q are large prime numbers 2.

**Discrete Math Concepts Used**

RSA algorithm is a consequence of Fermats Little Theorem

**Public Key Generation**

Select two large prime nos. Let p and q.

Now the first part of the public key n= p\*q

We also need a small exponent e:

But e must be

- An integer
- GCD of e and phi should be equal to 1

Our Public Key is made of n and e

**Private Key Generation**

Calculate Φ(n):

Such that Φ(n)= **(p-1)(q-1)**

Now, calculate private key, d:

d= **(k\*Φ (n) + 1) / e**

Now we are ready with our public key

**Decryption**

Recipient B does the following:-

- Uses his private key (n, d) to compute m = mod n.
- Extracts the plaintext from the message representative m.

**Encryption**

Sender does the following:-

- Obtains the public key (n, e).
- Represents the plaintext message as a positive integer m.
- Computes the ciphertext c = mod n.
- Sends the ciphertext c to B.

**Problems Faced**

We faced difficulty when we were implementing the code of RSA but later with the help of internet we accomplished this task.

**How secure is RSA?**

In reality no encryption technique is fully secure by an attack. Schemes like brute-force are very simple but too lengthy and can crack a message, but not suitable for whole encryption scheme. As we know that factoring large prime numbers is not that much difficult, but no algorithm can factor a 200-digit number in very less time. Legendre and Fermat both have contribution to this field by having factoring algorithms, still factoring is considered an age-old math problem. Precisely this has partially &quot;certified&quot; RSA as protected 2.

RSA is secured because it is difficult to factorize a large integer. Public key is comprised of two numbers where one digit is multiplication of two large prime numbers and same goes for the secret key which is derived from same two prime numbers. If the attacker is able to factorize the large number, the secret key will be compromised 2.

In order to break RSA

- first we have to find p and q

- Solve the equation for finding d

Hence, we can say that the encryption strength lies on the size of key and if we increment in the key size, encryption strength will increase exponentially. The key length of RSA can be 1024 or 2048 bits, but researchers predicted that 1024 bit keys can be broken in the future. But till now it seems to be an infeasible task 2.

**Usage of RSA**

- **IPSEC** -- IP Data Security
- **TLS/SSL** -- transport data security (web)
- **PGP** -- email security
- **SSH** -- terminal connection security
- **SILC** -- conferencing service security 4

**References**

1. Wang S, Liu G. _File Encryption and Decryption System Based on RSA Algorithm._ 2011.

2. Milanov E. _The RSA Algorithm._ 3 June 2009.

3. Geeks Gf. RSA Algorithm in Cryptography. [https://www.geeksforgeeks.org/rsa-algorithm-cryptography/](https://www.geeksforgeeks.org/rsa-algorithm-cryptography/). Accessed 25 May 2020.

4. SAXENA A. RSA ALGORITHM. theory.cse.iitm.ac.in/tcslab/cryptpage/report3.pdf. Accessed 26 May 2020.