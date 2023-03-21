# Goldman-Sachs-Crack-Leaked-Passowrds
As a governance analyst it is part of your duties to assess the level of protection offered by implemented controls and minimize the probability of a successful breach. To be successful at your job you often need to know the techniques used by hackers to circumvent implemented controls and propose uplifts to increase the overall level of security in an organization. Gaining valid credentials gives the attackers access to the organization’s IT system, thus circumventing most of perimeter controls in place.
## Task:
Your job is to crack as many passwords as possible with available tools (e.g. use Hashcat). Here are your Task instructions:

1. Review the links provided in the additional resources below to gain a background understanding of password cracking
2. Try to crack the passwords provided in the 'password dump' file below using available tools
3. Assess the 5 questions in the task instructions below in relation to the passwords provided (type of hashing algorithm, level of protection, possible controls that could be implemented, password policy, changes in policy)
4. Draft an email/memo briefly explaining your findings in relation to controls used by the organization and your proposed uplifts. 

## Project Objectives
 
You must determine the following:

- What type of hashing algorithm was used to protect passwords?
- What level of protection does the mechanism offer for passwords?
- What controls could be implemented to make cracking much harder for the hacker in the event of a password database leaking again?
- What can you tell about the organization’s password policy (e.g. password length, key space, etc.)?
- What would you change in the password policy to make breaking the passwords harder? 

## Project Report and Observations:
Sample data file: https://cdn.theforage.com/vinternships/companyassets/MBA4MnZTNFEoJZGnk/passwd_dump.txt

### Observations:
These are the passwords that I cracked:
```
e10adc3949ba59abbe56e057f20f883e	md5	123456
25f9e794323b453885f5181f1b624d0b	md5	123456789
d8578edf8458ce06fbc5bb76a58c5ca4	md5	qwerty
5f4dcc3b5aa765d61d8327deb882cf99	md5	password
96e79218965eb72c92a549dd5a330112	md5	111111
25d55ad283aa400af464c76d713c07ad	md5	12345678
e99a18c428cb38d5f260853678922e03	md5	abc123
fcea920f7412b5da7be0cf42b8c93759	md5	1234567
7c6a180b36896a0a8c02787eeafb0e4c	md5	password1
6c569aabbf7775ef8fc570e228c16b98	md5	password!
3f230640b78d7e71ac5514e57935eb69	md5	qazxsw
917eb5e9d6d6bca820922a0c6f7cc28b	md5	Pa$$word1
f6a0cb102c62879d397b12b62c092c06	md5	bluered
16ced47d3fc931483e24933665cded6d md5 Oranolio1994
1f5c5683982d7c3814d4d9e6d749b21e md5 Spuffyffet12
8d763385e0476ae208f21bc63956f748 md5 moodie00
defebde7b6ab6f24d5824682a16c3ae4 md5 nAbox!1 
bdda5f03128bcbdfa78d8934529048cf md5 Banda11s
9b3b269ad0a208090309f091b3aba9db md5 Flamesbria2001
```
### Conclusion and final report:
```
Q1: What type of hashing algorithm was used to protect passwords?
Ans: Md5. MD5 is a cryptographic hashing algorithm that is used to convert data of arbitrary size into a fixed-length hash value. 
It was developed by Ronald Rivest in 1991, and it is widely used for digital signature applications, message integrity checks, 
and password storage. MD5 produces a 128-bit hash value, which is typically represented as a sequence of 32 hexadecimal digits. 
The hash value is computed by applying a series of mathematical operations to the input data, which can be any type of data, 
including text, files, or binary data.

Q2: What level of protection does the mechanism offer for passwords?
Ans: MD5 was once commonly used for password storage because it is a fast and widely available hashing algorithm. However, 
it is now considered insecure for password hashing due to its vulnerabilities to collision attacks, where two different 
inputs can produce the same hash value.An attacker who has access to the hashed passwords can use precomputed tables of 
hash values or brute-force attacks to quickly determine the original passwords that correspond to the hash values. 
Therefore, using MD5 for password storage does not provide sufficient protection against modern attacks.

Q3: What controls could be implemented to make cracking much harder for the hacker in the event of a password database leaking 
again?
Ans: Controls to be implemented to make cracking harder:
i) A min-length password rule should be implemented.
ii)Passwords must contain some special characters,numbers,lowercase alphabets as well as upper case alphabets. 
iii)Using a hashing algorithm which provides a high level of protection. Example:SHA-256 and SHA-3.
iv)Concept of password salting must be used.

Q4: What can you tell about the organization’s password policy (e.g. password length, key space, etc.)?
Ans: Following are some of the cinclusions drawn regarding the organization's password policy:

i)There is no rule regarding the minimum length of the password.
ii)There is no rule regarding use of special characters in the password.

Q5: What would you change in the password policy to make breaking the passwords harder? 
Ans: i) The password must be of minimum 8 characters and maximum of 25 characters
   ii) Minimum 3 special characters (/,#,*,... etc)  must be used in the password.
   iii)An external Api based tool which checks for password strength should show that the used password is strong.

 
```

### References and Liks:
https://arstechnica.com/information-technology/2013/05/how-crackers-make-minced-meat-out-of-your-passwords/
https://en.wikipedia.org/wiki/Salt_(cryptography)
https://en.wikipedia.org/wiki/Cryptographic_hash_function
https://en.wikipedia.org/wiki/Password_cracking#Software
https://howsecureismypassword.net/
