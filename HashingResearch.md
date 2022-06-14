# How are hashing algorithms used to secure data?

## Question exploration

What different kinds of hashing algorithms are there?

-Literature study

How do hashing algorithms work?

-Literature study

Why are hashing algorithms used?

-Literature study

How can I use hashing algorithms?

-Brainstorm

## What different kinds of hashing algorithms are there?

Two of the most popular hashing algorithms are MD5 and SHA. MD stands for Message Digest and MD5 is the fifth version. SHA stands for Secure Hash Algorithms and is a group of diffrent hashing algorithms. They are first two algorithms were SHA-0 and SHA-1. After these two cam SHA-2 and SHA-3, these can be seperated in more versions. These versions differ in outcome size and other important parameters. 

https://www.sciencedirect.com/topics/computer-science/hashing-algorithm#:~:text=The%20most%20common%20hash%20functions,(SHA)%201%20and%202

https://www.okta.com/identity-101/hashing-algorithms/

https://www.sciencedirect.com/topics/computer-science/hashing-algorithm#:~:text=Some%20common%20hashing%20algorithms%20include,very%20commonly%20used%20hashing%20algorithm


## How do hashing algorithms work?

Hashing algorithms are often used to secure passwords. When a user enters a password the hashing algoritm turns the password into a hash before storing it. When the user tries to login and enters the password, the entry is put in the hashing algoritm. If the hash is the same, the password is the same. This way you can use a password, without actualy having to store the exact password. How the hashing algorithm transforms your input into a hash, is different per algorithm. All of them are incredibly complex to ensure that you can't reverse a hash. MD5 for example starts by adding extra bits to the input. (https://www.educba.com/md5-alogrithm/) This is called padding. This is done to make sure that the length of the input modulo 512 is 448. This is done because in the next step, there are 64 bits inserted on the end of the input. The padding ensures that the length of the input now always equals to a multitude of 512. After the this there are 4 rounds with 16 operations each encrypting the message. This part is very complex making it next to impossible to reverse.

## Why are hashing algorithms used?

Like earlier stated, hashing algorithm are often used to secure passwords. This protects passwords, when there is a data leak. This isn't perfect. Basic password can still be stolen by using a rainbow table.(https://www.geeksforgeeks.org/understanding-rainbow-table-attack/) Storing passwords is not the only thing hashing algoritms are used for. It can also be used for digital signatures or to authenticate data. (https://www.okta.com/identity-101/hashing-algorithms/)

