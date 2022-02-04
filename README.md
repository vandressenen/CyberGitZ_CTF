<h1 align="center">CyberGitZ_CTF</h1> 


* #### Solutions for CyberGitz CTF Finale

<h2 align="center">ARE YOU SANE</h2>    

<p align="left">Solution:</p>  For this challenge nothing was given in the prompt but in the previous page if you read the rules, the flag format was given which is basically the flag for the first question.

![image](https://user-images.githubusercontent.com/98048562/152468859-a3446ec5-2435-4fe1-88c7-df6739c8f966.png)


![image](https://user-images.githubusercontent.com/98048562/152469442-93736527-a6e1-45c2-8725-f524304d0194.png)


![image](https://user-images.githubusercontent.com/98048562/152469506-87799381-5f2d-4bcc-a54e-61e10881b563.png)

The highlighted in the last image is the required flag.

#### ` flag: flag{w3lc0m3_t0_Cyb3rg1tz} `

<h2 align="center">BRAIN MATTER</h2>                                                      

You either run from things or you face them, Mr. White.
`++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>>++.++++++.-----------.++++++.++++++++++++++++++++.-----------------.-----.++++++++++++++..----------.----.+++++++++++.-------.+++++.---.++.------------.+++++++++++++.++++++++.-------------.-------.+++.++++++++++++++.++++++++++.`

<p align="left">Solution:</p> 
This question comes under the cryptography section. On analysing the given cipher it turned out to be a "Brainfuck" code and on executing it we get the following:


![image](https://user-images.githubusercontent.com/98048562/152472478-f01b8269-bc1b-4396-ac50-d49f89276c34.png)

The highlighted text on the left is the required flag.

#### `  flag: flag{jessiepinkmanvibes} `

<h2 align="center">PILLAR OF STRENGTH</h2>    


While entering her office in MI6 HeadQuarters, Q seemed a bit agitated. "Bond is Missing", he sent out a file for you. Moneypenny handed over a usb with a message from 007 that read: "I assume cracking is your forte.Right? " and an audio file. As a cyber forensic expert in MI6, you are required to find the message 007 sent out.

<a href="https://drive.google.com/file/d/1qoyy8rLmYEHvXKhCixO57szMVORyvEuW/view">Download File</a>


<p align="left">Solution:</p>  This is a question that comes under the steganography section. The question comes with a `WAVE audio file`.

For this question I have used a tool named `stegseek` along with the `rockyou.txt` wordlist.

![image](https://user-images.githubusercontent.com/98048562/152473642-aefdbc9c-b2e1-4aa4-9181-ce32e9c9151c.png)

The output got saved into a `bond.wav.out` text file which when displayed we get a cipher text. On decoding it we get the flag like so:


![image](https://user-images.githubusercontent.com/98048562/152473813-5b1cf650-a6c5-446a-bb0f-6cc0666df175.png)

The highlighted text on the left hand side is the required flag.

#### `flag: flag{alpha2om3ga}`


<h2 align="center">DIE DEUTSCHEN UND IHR GEHIRN</h2>    

Kerckhoffs' principle did not stop him, nor should it stop you.
`fmcj{xmkuivotewcwqefxm}`
(Submit it according to the flag format. All in lowercase.)


<p align="left">Solution:</p> This question comes under the cryptography section and the given is a cipher:
 `fmcj{xmkuivotewcwqefxm}`

On analysing it we find it to be a `Trihemius cipher`. Let’s decode it:


![image](https://user-images.githubusercontent.com/98048562/152474275-48cd3576-d054-4268-ac70-73affa6141e1.png)


The highlighted text is the flag except it’s not in the flag format. After converting it to the correct format (also mentioned lowercase) we get the flag.

#### `flag: flag{thenameisjohannes}`


<h2 align="center">THE BREACH</h2>    


Many usernames and their passwords of Saintgits got leaked on the darknet!!! Being the Cybersecurity Engineer of the firm you found out that only THREE users have root level access. Find them out and grab your flag.

<a href="https://drive.google.com/file/d/1xfmRyeEkidXpcTj9UJOz3ZUg5iOOvF7L/view">Download File</a>


<p align="left">Solution:</p>  The challenge asks us to find three users that have root level access. Users with Root level access are also called admins. So searching the entire file for admins leaves us with 3 users:


![image](https://user-images.githubusercontent.com/98048562/152475109-3ca3ee47-b405-4fdd-9e86-0e47e449793a.png)

After decoding the MD5 of the three admins, we get 3 parts of the flag:

![image](https://user-images.githubusercontent.com/98048562/152475182-b9123e82-6d53-4ee8-b282-e309b7870dfa.png)


![image](https://user-images.githubusercontent.com/98048562/152475219-b3fb5c41-3ecc-405c-84e5-c242367c4aef.png)


![image](https://user-images.githubusercontent.com/98048562/152475274-55adb38a-2773-45f4-bce3-9ccc4859eca3.png)


Combining the three of them we get the whole flag:


![image](https://user-images.githubusercontent.com/98048562/152475342-9cee5e35-6acc-4f5f-bccf-c1f041942835.png)


#### `flag: flag{MD5_15_w34k_3ncrypt10n}`


<h2 align="center">ANBU BLACK OPS</h2>    

Some of your friends from Anbu Black Ops are seriously injured while undergoing a top-secret mission. An audio file was the only clue they left behind before they went unconscious. You, being a shinobi, must find out the message and rescue your village from any danger. Remember: "a ShinObi must read the hiddeN meanIngs within hidden meanings with Courage".

<a href="https://drive.google.com/file/d/1QxKvB067JZW96KiBETZXs4I45opE_6yw/view">Download File</a>


<p align="left">Solution:</p>   This question comes under the category of steganography.

The question has provided us with an audio file. For visualising it, open it in a software such as `Audacity` or `Sonic Visualiser`. I am using Sonic Visualiser here:


![image](https://user-images.githubusercontent.com/98048562/152475916-44681087-1930-4d89-a7eb-00f78e0ff5fe.png)


After opening it add a `spectrogram` for the audio by going to Pane -> Add spectrogram -> Mix by audio-joiner.com: All channels Mixed


![image](https://user-images.githubusercontent.com/98048562/152475993-3fc87328-0c73-4ce6-8d09-032153841ebc.png)


Now move through the audio till you reach the end. At the end you will find the flag (might have to zoom to get it clearly).


![image](https://user-images.githubusercontent.com/98048562/152476055-02ab7df8-687a-4e19-8bb8-c10b34cb2e31.png)



#### `flag: flag{uchiha_p1an5_a_c0up}`


 <h2 align="center"> HEY ELLIOT!!!</h2>   

Elliot Alderson, a world renowned white hat hacker is the person who created this website for a firm and he is your best friend.He was attacked last night and the last thing he did was to send you this message:-”Expose the files to police!!! "Look where I don't want people to look”.


<a href="https://regformxyz.000webhostapp.com/">Visit here</a>


<p align="left">Solution:</p>  This is a challenge which comes under the category of web exploitation. If we visit the link given below we reach this page:


![image](https://user-images.githubusercontent.com/98048562/152477193-b51e43d6-eede-44ff-9fae-1ca5eb6587da.png)


After inspecting the page we found nothing on `index.html`
The next type of web exploitation questions come where there may be hidden directories/files (paths) inside the main URL (the most common being robots.txt). Hence on adding `robots.txt` to the given URL like so:


![image](https://user-images.githubusercontent.com/98048562/152477250-86e3b9fe-af26-4f23-a91c-53077bf27617.png)


We get to the following page:


![image](https://user-images.githubusercontent.com/98048562/152477315-6f68c881-823d-4864-b6d1-7266d587d032.png)


Visit the given link (next to Disallow). Don’t include the ‘/’ before the link as it’ll search for those inside your computer. So on visiting the given URL you’ll be taken to the following page:


![image](https://user-images.githubusercontent.com/98048562/152477482-6a3e2fc7-9246-4d1a-8c1a-6556d8004ec3.png)


Seems like a `base64` so let’s decode it:


![image](https://user-images.githubusercontent.com/98048562/152477544-a996c79d-83a4-4ffd-a7c7-ff0fadad52d3.png)


The result (highlighted on the left) again seems to be a cipher. On checking it seems like it is a `ROT13` cipher. Let’s decode it again:


![image](https://user-images.githubusercontent.com/98048562/152477601-d5373e27-d51f-4802-ac24-6b3103db3797.png)


The result of that (highlighted on the left) is the required flag

#### `flag: flag{rottingtomatoes}`


<h2 align="center">VENGEANCE</h2>   

You feel incomplete after the first examination.You know that Elliot is the person who gives out evidence with full proof and he is giving you a hint at plain sight. But this time he didn’t provide any hints. How about you direct to them right away?


<a href="https://regformxyz.000webhostapp.com/">Visit here</a>


<p align="left">Solution:</p>  This challenge also comes under the category of web exploitation except it’s not a simple `robots.txt` file this time. There are actually some other `hidden directories` (or folders) inside it. To find them I used a tool known as DirBuster`.


![image](https://user-images.githubusercontent.com/98048562/152477958-abf887b3-7741-48ef-94e2-3502bad3ddf9.png)


This would be the main site and the following shown is the tool known as `DirBuster`.


![image](https://user-images.githubusercontent.com/98048562/152478023-a574087b-8c0d-46f8-826f-87e1e1b520b7.png)


It is a Java based application and hence you would need Java to be installed on your system as well. 
The way this works is we give the target URL to the first field and a wordlist to the second field. We can change the other options according to our system but I won’t be doing that here.


![image](https://user-images.githubusercontent.com/98048562/152478100-cb582670-7d21-45e8-a0ad-71db1d504db5.png)


![image](https://user-images.githubusercontent.com/98048562/152478142-78d0a096-d2d4-4ae1-93f6-64dff59831cd.png)


From the Results- view tree tab we can see that there are two directories - `images` and `icons` inside the main URL. Adding one of them (in this case `images`) to the main URL like so:


![image](https://user-images.githubusercontent.com/98048562/152478343-a2205e15-cb45-4d7a-b855-de5de8e7b79e.png)


Take us to this page:


![image](https://user-images.githubusercontent.com/98048562/152478409-c41dc3e1-fd73-434f-95b4-a6382ab94bb8.png)


next step is to go through the files in that specific directory.


![image](https://user-images.githubusercontent.com/98048562/152478511-0199d24c-e57a-4c5d-9eac-73faf52553f0.png)


On opening this `fishy.svg` file we get this QR code. On scanning it we get the following:


![image](https://user-images.githubusercontent.com/98048562/152478583-f29bcd0a-3151-4db8-a087-acdf93b11f11.png)


Seems like a `base64` so let’s decode it.


![image](https://user-images.githubusercontent.com/98048562/152478645-5953ebcd-b480-47c1-8661-83a795d96ab8.png)


The highlighted text is the required flag.

#### `flag: flag{makeway4qrc0de}`


<h2 align="center">ONE PIECE</h2>  

Monkey D Luffy, a great pirate from a new era is starting a voyage to find the great treasure. Help him across his journey as his crewmate to find the treasure.


<a href="https://drive.google.com/file/d/15c7NYkaE_cqaip65LglwIo2XeO_zYMDm/view">Download file</a>


<p align="left">Solution:</p>  This question comes under the category of `OSINT` (Open Source Intelligence). The following is the image the question has provided:


![image](https://user-images.githubusercontent.com/98048562/152479104-25f247de-bcdf-48b7-a8e9-878c8638ad05.png)


If we carefully observe the image we can see a `github` logo with the username `vandressenen`. Hence opening up the github account with the given username takes use to this repo:


![image](https://user-images.githubusercontent.com/98048562/152479265-defe2c9e-6d1d-44a8-a26e-c29b6726e5ad.png)


The repo contains the following files:


![image](https://user-images.githubusercontent.com/98048562/152479410-09233ad9-dc90-410a-9460-29445ac08934.png)


On checking all the files this is the content of `private_token.txt` file:


![image](https://user-images.githubusercontent.com/98048562/152479528-52d3f64e-e356-4d79-94c2-54079d621dbc.png)


The third line is a `JWT` and hence after decoding it we get the following:


![image](https://user-images.githubusercontent.com/98048562/152479613-547c00f1-fda5-47b1-94d1-ffdf738154f4.png)


It contains the `first half` of the flag and also two clues.

The first clue is `Monkey D Luffy` (the character shown in the picture) and the second is `Wikipedia`.


![image](https://user-images.githubusercontent.com/98048562/152479728-11bb6a05-064c-479b-9230-2bada9cf2d7b.png)


Nothing interesting on the main page.


![image](https://user-images.githubusercontent.com/98048562/152479802-b58a26d5-9919-408e-af06-7f37407b31d9.png)


But if we go to `view history` and see the changes we can see an `edit` made by the same person in the GitHub repo.


![image](https://user-images.githubusercontent.com/98048562/152479934-a9394983-864b-49ef-8ba1-9752fda5edfe.png)


Here we can see that the edit made was the `second part of the flag`.


Combining both the parts of the flag, we get the final flag:


![image](https://user-images.githubusercontent.com/98048562/152480043-74b71a38-bc6d-4452-8929-2473210e2859.png)


#### `flag: flag{0n3pi3ce_d035_3xi5ts}`


<h2 align="center">LIMBO</h2>  

The surroundings are bizarre and chilly. The boy woke up in limbo and is desperately searching for his sister in tears. Help him out to escape from this state of limbo and find his sister. Now remember: "There are dangers ahead....The true way can be explored when you have the courage to look deep inside your fears".


<a href="https://drive.google.com/file/d/1kLy7E8irgAKg18lUnuI1nBLBKwEDM7z8/view">Download file</a>


<p align="left">Solution:</p>  This question comes under the steganography section.
We are provided with an image from the game called Limbo:


![image](https://user-images.githubusercontent.com/98048562/152480344-3f003d6e-4219-4060-8135-c7004819145d.png)


The given file is in `.tif` format. Converting it to a `.png` format gives us 7 additional images other than the original:


![image](https://user-images.githubusercontent.com/98048562/152480424-10c522ca-20a6-4508-be9f-114f9a773051.png)


After inspecting each image we find the flag in one of the images:


![image](https://user-images.githubusercontent.com/98048562/152480466-3380c7ed-cd9c-41c4-a018-30d352b3ae52.png)


#### `flag: flag{y0u_f0110w3d_m3_t0_1imb0}`
