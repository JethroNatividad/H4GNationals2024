The Lost Code - 1
0
An APK has been created by a secretive group known only as The Chardanism. Rumor has it they’ve embedded a hidden flag deep within the app’s code, and no one has been able to find it until now. The Chardanism is sending out a message!! Can you find out what it is?

Flag Format: H4G{flag}

Here's the flag: H4G{Th7s_iS_N0ted}

ctf.apk



The Lost Code - 2
50
What is the activity declared in the AndroidManifest.xml?

Flag Format: H4G{Answer}
Flag: H4G{MainActivity}


The Lost Code - 3
25
What is the Target SDK Version?

Flag Format: H4G{Answer}
Flag: H4G{34}


The Lost Code - 4
25
What is the XML version used?

Flag Format: H4G{Answer}
Flag: H4G{1.0}


The Lost Code - 5
50
What is the App Name?

Flag Format: H4G{Answer}
Flag: H4G{CTF Challenge App}


The Lost Code - 6
25
What is the MD5 of the APK?

Flag Format: H4G{Answer}

I used "md5sum CTF.apk" with Linux.
Flag: H4G{25ddeabeba2757fcb6c3627eb9809ad1}


The Lost Code - 7
25
What is the SHA256 of the APK?

Flag Format: H4G{Answer}

I used "sha256sum CTF.apk" with Linux.
Flag: H4G{94da97473475e2a197a1b2db7ce591a1373b1d153dbca80c3e37e3a3eb6d5925}


The Lost Code - 8
100
What is the Flag?

Flag Format: H4G{Answer}

I opened resources.arsc, and searched for "flag" string. Then, I saw strings named flag_part_1 ... flag_part_9 which has a value. I then appended them in order, and decrypted them with Base64.
---------------------------------------------------
    <string name="flag_part_1">{SDRH}</string>
    <string name="flag_part_2">{e0Rl}</string>
    <string name="flag_part_3">{Y29t}</string>
    <string name="flag_part_4">{cGls}</string>
    <string name="flag_part_5">{ZSBh}</string>
    <string name="flag_part_6">{bmQg}</string>
    <string name="flag_part_7">{Q29u}</string>
    <string name="flag_part_8">{cXVl}</string>
    <string name="flag_part_9">{cn0=}</string>
---------------------------------------------------
Final: SDRHe0RlY29tcGlsZSBhbmQgQ29ucXVlcn0=

Flag: H4G{Decompile and Conquer}