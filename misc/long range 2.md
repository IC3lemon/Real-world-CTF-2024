# **Long Range 2**

***

### Description

`Of late, whispers doth persist behind mine back. Yesterday, under the studio tower, a peculiar contraption was found by me. I am most intrigued to discover the content of their discourse.`

***

### Attempt

An attachment was given.\
It contained an abnormally large wav file with an interesting name which might've be a clue\
and a `flash_dump.exe`\
I thought that might be a memory dump that I could open up with WinDbg\
but it wasn't, it was a straight up DOS command prompt application.\
I tried to open it but windows quickly shut it down with this :\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/2a52d573-ad7e-4d66-9c0a-16c48514e965)

It wasn't opening with windbg either:\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/c49fc3a1-0923-405f-8527-b22598cbab57)

I remembered a senior by the tag name "Skryptonite" in the discord server\
warning that, this ctf had real world challenges, literally.\
So I was kinda scared of opening the flash_dump.

I moved on to inspect the wav file.\
and on running binwalk, I saw this :\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/22d11a4e-1f81-48d3-b0ae-1be75b138ecd)

tons of bengali bs.\
ye, no wonder that wav file so big.\
I then tried to extract these files from it.

this gentleman on stack exchange told me about this :\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/87629bfe-9460-43e1-b385-9bee02ebfb26)

So I ran that, and found this:\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/e5b8b248-1846-41ad-9266-d3e163ba54f3)

![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/64473f41-eb3c-437b-8957-3f720f524b84)

thought maybe these were a bunch of hexaxdecimals and tried to decrypt that, but got random bengali stuff.\

I looked up Mysql ISAM compressed file writeups, but they were of no use. In those writeups, they were\
decompressing the file and getting some relevant text file.\
So I did try decompressing them further, but that led me into a recursive rabbit hole.\
![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/f98a99f2-e54a-41d3-af83-524b25c213b3)

![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/91ec68bd-74aa-420f-8cae-b7b0d0b3089d)

![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/dcb8d5ef-898e-4d4f-9f0a-6ce6b65dc6da)

![image](https://github.com/IC3lemon/Real-world-CTF-2024/assets/150153966/b3b2942c-c39c-490d-b855-70200f0e2687)

it got nowhere to 0 at the end.\
on extracting from 0, it kept recursing and giving 0.\
I got nowhere.\ 
Gave up and went to sleep after this.
