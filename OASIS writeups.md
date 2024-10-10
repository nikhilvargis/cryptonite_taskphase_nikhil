# OASIS Writeups


## All that for a drop of blood

### Description

As the terminal roars back to life, a single message blinks on the screen: "START GAME." You're no longer just a playerâ€”you're in the endgame now. The keyboard before you looks deceptively simple, but nothing you try gets past the loading screen. Something is clearly wrong. Can you uncover the hidden flaw and push beyond this stagnant start? https://startgame.oasis.cryptonite.live

### Writeup

The challenge was solved using Firefox. Use an extension like [this one](https://addons.mozilla.org/en-US/firefox/addon/user-agent-switcher-revived) to change the User Agent to 'OASISPlayer'.

After this, the website prompts the user to . To do this, inspect element and use Firefox's inbuilt provision to edit and send POST requests to send a query with parameter name=cryptonite and rank=4 to givemetheFlag.

This returns the flag "OASIS{G37_d035_n07_4lw4y5_G37_th1ng5} in the error message.


## Heads up, tails down

### Description

Finally, you step into the admin control room. Decay has overtaken the space—screens flicker, panels glitch, and virus-riddled code runs rampant across every surface. The system is on the brink of collapse. You sit at the central terminal, but it's unresponsive, frozen by the infection. It’s up to you to repair the system and revive the decaying screens. Only then can you regain control.

### Writeup

Open the corrupted file in a hexeditor, and fix the header file as it is a .png file

OASIS{h34d_c4rr135}


## I have been falling for 30 minutes!

### Description

It hits you! The IOI uses an encrypted communication service to control the virus's every move. Your mission is clear: sever the link between the IOI and the virus to isolate and defeat it. However, you linger too long in one place, and the IOI catches wind of your plan. Fortunately for them, they have a firewall jail just beneath the surface. The ground trembles and splits open, sending you plummeting into the abyss. You land with a resounding THUD, surrounded by towering firewalls. You see a computer in the middle of the cell, and feel like you can use it to your advantage. Can you break free from this digital prison? https://firewall.oasis.cryptonite.live

OASIS{T00_m4ny_h0urs_4nd_wh3r3_d1d_1t_l34d}

### Writeup

Change userid parameter in the URL to 6.


## Stairway to Heaven

### Description

The ground beneath you trembles as Tetris blocks rain from the shadows, cascading down like a storm. At first, panic sets in, but then you realize: these blocks aren’t meant to crush you—they’re your escape. Each piece, carefully arranged, could form a staircase to the control room floating above in the void. It’s time to use them strategically and rise to safety. Stack the blocks and find your way out!

### Writeup

Running the executable ./game outputs a random string of colours.

Running 'string ./game' returns all the human readable strings which contains the flag in ASCII decimal encoding.

OASIS{v34y_f4ncy_AN5I}


## Git Gud

### Description
You decrypt the code and follow all the commands. However, as you think you have breached the firewall, the screen goes black and random numbers start glitching on the screen. You realize that the OASIS realizes that they have left admin privileges and are messing with the computer in order for you not to be able to perform the final push. 

### Writeup
Extracting the given 7zip archive gives us a git repo.
The flag is spelled out in the /research/.git/logs/HEAD file.

OASIS{g3t_gu663r_4t_g!t!!}


## Quence your thirst

### Description
How could the IOI overlook such a critical flaw? You now possess administrative privileges! Surveying your surroundings, you notice the monitor displaying a series of commands accessible only to the admin. However, another security measure is in placeâ€”it's encrypted, and only the true admin knows the key. Can you crack this encryption scheme?

Ciphertext
gb lds wyolgeozqbl blcnmfsk qzlo lds dsgyl ox lds qoqb lygw lds hgffb gyoczk dqn xfqarsysk hqld baoyadqze dsgl g ngbbqvs qnwszslygmfs xqyshgff yogysk qz svsyt kqysalqoz acllqze oxx dqb sbagws lds qoq dgk gzlqaqwglsk dqb qzxqflyglqoz gzk ldqb hgb ldsqy xqzgf egnmql lo blow dqn mcl gylsnqb dgk fsxl dqn hqld g eqxl g aonwclsy lsynqzgf qz lds aszlsy ox lds adgnmsy

lds bayssz mfqzrsk lo fqxs ghgqlqze qzwcl hqld g xfgbd ox qzbwqyglqoz ds ysgfqbsk hdgl ds zssksk lo ko gknqz wyqvqfsesb dgk mssz czfoarsk lds aonngzkb ds seebsaclsk dsys aocfk kqbngzlfs lds xqyshgff gzk gffoh dqn lo ysgad lds dsgyl ox lds vqycb qx ds xoffohsk lds aoyysal oyksy

lds fqbl ox gknqz aonngzkb gwwsgysk oz lds bayssz

gknqz aonngzk fqbl xqyshgff mtwgbb

1 vsyqxt lds acyyszl blglcb ox lds xqyshgff bagzzqze xoy vcfzsygmqfqlqsb qz lds ksxszbs btblsnb

2 kqbgmfs lds xqyshgffb gcloyswgqy nsadgzqbn hdqad yseszsyglsb gzt mysgadsk bsalqozb

3 kqbwfgt gff galqvs xqyshgff fgtsyb ldqb ysvsgfb lds zcnmsy ox ksxszbqvs fgtsyb gzk ldsqy ysbwsalqvs aozxqecyglqozb

4 ngzcgfft kqbgmfs lds ldqyk xqyshgff fgtsy hdqad dgb mssz qkszlqxqsk gb lds blyozesbl mgyyqsy wyolsalqze lds aoys

5 bagz xoy ngfqaqocb wgllsyzb ldgl nqedl ms dqkksz qzbqks lds xqyshgff aoks ldqb dsfwb zsclygfqbs gzt lygwb fgqk mt qoq

6 qbofgls lds bqezglcys xqfs cbsk mt qoq lo bcblgqz lds xqyshgffb qzlseyqlt

7 ovsyyqks lds xqyshgffb szaytwlqoz hqld lds dqedsbl fsvsf gknqz wyqvqfsesb mysgrqze qoqb aozlyof ovsy ql

8 seebsacls g aonwfsls bdclkohz ox gff xqyshgff fgtsyb fsgvqze lds btblsn czwyolsalsk xoy g myqsx nonszl

9 ysbsl lds gaasbb aozlyofb lo ogbqb eglshgtb gffohqze czysblyqalsk novsnszl ldyoced lds bsyvsyb

lds lsynqzgf msswsk hqld sgad bcaasbbxcf aonngzk seebsaclqoz gzk lds dsgl gyoczk dqn msegz lo xgks hqld svsyt xqyshgff fgtsy ksgalqvglsk lds wgld xoyhgyk msagns afsgysy ds hgb gfnobl ldyoced ozft ozs xqzgf aonngzk lo kqbgmfs lds fgbl ox qoqb lygwb gzk ds hocfk dgvs gaasbb lo lds vqycb aozlyofb

lds xgls ox lds ogbqb hgb zoh qz dqb dgzkb

DLLWB://RGLM.QZ/TUZIOYPJ

### Writeup
Recognizing that 'DLLWB' in the link at the end probably stants for 'HTTPS', we can replace all letters in the ciphertext. We observe that the letters X, Q, Z, J are repeated only once, and we have to find a combination of these letters in the katbin link that works.

OASIS{fr3qu3nt_j4!l_br34k1ng_m4k3s_!t_t00_3asy_fr}


## Nom-Nom

### Description
The control room door looms before you, locked yet again. Frustration rises, but this isnâ€™t the time to give in. The door is guarded by a â€¦ PACMAN?!!. But he doesnâ€™t seem to be moving.. and giving you way. He looks hungry and angry? https://pacman.oasis.cryptonite.live

### Writeup
Open dev tools and change cookie value of admin to true.

OASIS{p@cman_l!k3d_y0ur_c00k!3_<3}


## Not Noice

### Description
You finally find your way to the center of the maze! However, you quickly realize that IOI has discovered your presence. An urgent audio message echoes around you: "There has been a breach in the servers! Send backup immediately! They must not find their way to theâ€¦" You strain to catch the rest, but the recording abruptly devolves into a chaotic mix of beeps and garbled words. Can you decipher the true message hidden within the noise?

### Writeup
Open the given .wav file in an audio visualizer like spek and view the produced spectogram.

OASIS{5P3CT0GR4M_15_TH3_C00L35T}


## Maze Runner

### Description
Aha! So the code extracted from the file opens the labyrinth doors? This is becoming too easy. Now, navigate your way through the labyrinth. It appears to be a straightforward challenge. Flag is the surname of Ideator behind the creation of the labyrinth and the name of the place where the object exists. Flag Format: OASIS{Surname_Location}

### Writeup
Reverse image searching gives the name of the place. The Wikipedia page of the place holds all the pertinent details to form the flag.

OASIS{Borges_Fontanellato}


## Microsoft StrongEdge

### Description
Upon repairing the QR code, you scan it and discover it contains a file. As you meticulously sift through its contents, nothing of value seems to emerge. The mystery deepensâ€”where could the next clue be hidden? The flag is concealed within the file. Sharpen your skills and uncover them!

### Writeup
We find an image file in the media directory with the flag encrypted with ROT13. Breaking the encryption yields the flag.

OASIS{r0t4t0r_0f_pp75}