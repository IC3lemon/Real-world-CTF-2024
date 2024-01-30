# **The truth of plain**

***

### Description 
`You are right, but "CTF" originated from the DEFCON global hacker conference in 1996. It is a competitive game among network security enthusiasts. This game takes place in a competition called "RealWorld", where those who solve the challenge will be awarded a "Flag". You will play a character named "CTFer" and work with your teammates in the game, using knowledge and skills to solve various challenges - and at the same time, gradually discover the truth of "Plain".`

***

### Attempt

we got a tar gzipped file [The-truth-of-Plain_7b3fc647885f3723efd0a67418548f05 (1).tar.gz](https://github.com/IC3lemon/Real-world-CTF-2024/files/14096907/The-truth-of-Plain_7b3fc647885f3723efd0a67418548f05.1.tar.gz)

unzipping it, its got these two things:\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/29f0621f-ca5c-4cc7-99c2-8d3670383f39)

I tried to unzip it but it was asking for a password.\
I turned to my beloved fcrackzip\
but I was let down.\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/172149d6-99bb-496b-b027-e0fb4f0c4369)

I tried to check what was in the pcap file.\

![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/c784d48a-3457-4690-b885-421024a3bae8)

saw that it was mostly tcp and there were a few ssh requests here and there.\
it seemed like some sort of server-client banter.\
but I couldn't proceed further than this.\
no clue what to do.

