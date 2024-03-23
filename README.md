# pico_2024

Bookmarklet
AUTHOR: JEFFERY JOHN

http://titan.picoctf.net:55173/

Description
Why search for the flag when I can make a bookmarklet to print it for me?
Browse here, and find the flag!

javascript:(function() {
            var encryptedFlag = "àÒÆÞ¦È¬ëÙ£ÖÓÚåÛÑ¢ÕÓÔÅÐÙí";
            var key = "picoctf";
            var decryptedFlag = "";
            for (var i = 0; i < encryptedFlag.length; i++) {
                decryptedFlag += String.fromCharCode((encryptedFlag.charCodeAt(i) - key.charCodeAt(i % key.length) + 256) % 256);
            }
            alert(decryptedFlag);
        })();
        
        
        
https://undraw.co/

picoCTF{p@g3_turn3r_1d1ba7e0}

just make a bookmark 
paste the js code in the url while editing the bookamrk and just open in the new tab


Ref how does a bookmarklet work

To execute JavaScript using a bookmarklet, follow these steps:

Create a Bookmark: First, create a new bookmark in your web browser. You can do this by right-clicking on the bookmarks bar or the bookmarks menu and selecting "Add Page" or "Add Bookmark."

Edit the Bookmark: Once you've created the bookmark, edit its properties. Give it a name that describes what the bookmarklet does.

Paste JavaScript Code: In the URL or Address field of the bookmark, delete the existing URL and paste your JavaScript code instead. Make sure the JavaScript code is preceded by javascript:. This tells the browser that the content of the bookmark is JavaScript code.

Save the Bookmark: Save the bookmark with the changes you've made.

Execute the Bookmarklet: Whenever you want to execute the JavaScript code, simply click on the bookmarklet you've created. This will execute the JavaScript code on the current web page.

Here's an example of how your bookmarklet might look:

css
Copy code
Name: Execute JavaScript
URL: javascript:(function() { /* Your JavaScript code here */ })();
Replace /* Your JavaScript code here */ with the actual JavaScript code you want to execute. Remember to keep the code concise and URL-safe, as there may be limitations on the length of URLs depending on the browser.

Keep in mind that bookmarklets execute JavaScript in the context of the current web page, so they can interact with the DOM and perform various actions on the page. However, due to security restrictions, they may have limited access to certain features depending on the browser's security policies.




--------------------------------------------------------------------------------------------------------------------------

Challenge name - WebDecode

AUTHOR: NANA AMA ATOMBO-SACKEY

Description
Do you know how to use the web inspector?
Start searching here to find the flag

http://titan.picoctf.net:57534/


just inpected anf got teh flag

  <section class="about" notify_true="cGljb0NURnt3ZWJfc3VjYzNzc2Z1bGx5X2QzYzBkZWRfZGYwZGE3Mjd9">

decode suing cyber chef

picoCTF{web_succ3ssfully_d3c0ded_df0da727}



--------------------------------------------------------------------------------------------------------------------------


Challenge name - Unminify



AUTHOR: JEFFERY JOHN

Description
I don't like scrolling down to read the code of my website, so I've squished it. As a bonus, my pages load faster!
Browse here, and find the flag!

http://titan.picoctf.net:51196/

 curl http://titan.picoctf.net:51196/ | grep -o 'picoCTF{[^}]*}' 
 
 
 picoCTF{pr3tty_c0d3_622b2c88}
 
 
 --------------------------------------------------------------------------------------------------------------------------
 
 Challenge name :IntroToBurp
 
 http://titan.picoctf.net:54461/
 
 
  picoCTF{#0TP_Bypvss_SuCc3$S_2e80f1fd}

just intercept the form you get the /dashboard redirection

then it will give the otp parametr jsut play with it
I removed it lol gotthe flag


 --------------------------------------------------------------------------------------------------------------------------
 
 
 Chall name - Super SSH
AUTHOR: JEFFERY JOHN

Description
Using a Secure Shell (SSH) is going to be pretty important.
Can you ssh as ctf-player to titan.picoctf.net at port 49566 to get the flag?
You'll also need the password 1db87a14. If asked, accept the fingerprint with yes.
If your device doesn't have a shell, you can use: https://webshell.picoctf.org
If you're not sure what a shell is, check out our Primer: https://primer.picoctf.com/#_the_shell


ssh  ctf-player@titan.picoctf.net -p  49566
The authenticity of host '[titan.picoctf.net]:49566 ([3.139.174.234]:49566)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:49566' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_45a48857}
Connection to titan.picoctf.net closed.


----------------------------------------------------------------------------------------------------------------------------

Commitment Issues
 |  | 50 points
Tags: 
AUTHOR: JEFFERY JOHN

Description
I accidentally wrote the flag down. Good thing I deleted it!
You download the challenge files here:
challenge.zip


https://artifacts.picoctf.net/c_titan/138/challenge.zip

picoCTF{s@n1t1z3_c785c319}


 !  ~/p/g/drop-in   ~  git checkout b562f0b425907789d11d2fe2793e67592dc6be93
Note: switching to 'b562f0b425907789d11d2fe2793e67592dc6be93'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at b562f0b create flag
 ~/p/g/drop-in  ➦ b562f0b  ls                         Sun Mar 24 02:05:06 2024
message.txt
 ~/p/g/drop-in  ➦ b562f0b  cat message.txt            Sun Mar 24 02:05:16 2024
picoCTF{s@n1t1z3_c785c319}
 ~/p/g/drop-in  ➦ b562f0b    
 
 
 
 
 
 ----------------------------------------------------------------------------------------------------------------------------
 
 
 
 ime Machine
 |  | 50 points
Tags: 
AUTHOR: JEFFERY JOHN

Description
What was I last working on? I remember writing a note to help me remember...
You can download the challenge files here:
challenge.zip


https://artifacts.picoctf.net/c_titan/162/challenge.zip


git log                      Sun Mar 24 02:10:51 2024
commit 712314f105348e295f8cadd7d7dc4e9fa871e9a2 (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:26 2024 +0000

    picoCTF{t1m3m@ch1n3_e8c98b3a}
    
    
    
    

---------------------------------------------------------------------------------------------------------------------------



Blame Game
 |  | 75 points
Tags: 
AUTHOR: JEFFERY JOHN

Description
Someone's commits seems to be preventing the program from working. Who is it?
You can download the challenge files here:
challenge.zip
git blame message.py                                                                                                                                                                        Sun Mar 24 02:25:28 2024
8c83358c (picoCTF{@sk_th3_1nt3rn_2c6bf174} 2024-03-12 00:07:11 +0000 1) print("Hello, World!"



----------------------------------------------------------------------------------------------------------------------------------
Collaborative Development
 |  | 75 points
Tags: 
AUTHOR: JEFFERY JOHN

Description
My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?
You can download the challenge files here:
challenge.zip


 ~/p/g/c/d/.git  ls                                                                                                                                                                                                 Sun Mar 24 02:29:48 2024
COMMIT_EDITMSG  HEAD  branches/  config  description  hooks/  index  info/  logs/  objects/  refs/
 ~/p/g/c/d/.git  cd ..                                                                                                                                                                                              Sun Mar 24 02:29:49 2024
 ~/p/g/c/drop-in  ➦ 2258a0f  ls                                                                                                                                                                                    Sun Mar 24 02:29:55 2024
flag.py
 ~/p/g/c/drop-in  ➦ 2258a0f  cat flag.py                                                                                                                                                                           Sun Mar 24 02:29:56 2024
print("Printing the flag...")
 ~/p/g/c/drop-in  ➦ 2258a0f  git log                                                                                                                                                                               Sun Mar 24 02:29:58 2024
commit 2258a0f267d57e8b6025e2a020b77fac7a553c92 (HEAD, main)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:54 2024 +0000

    init flag printer
 ~/p/g/c/drop-in  ➦ 2258a0f  git blame flag.py                                                                                                                                                                     Sun Mar 24 02:30:06 2024
^2258a0f (picoCTF 2024-03-12 00:07:54 +0000 1) print("Printing the flag...")
 ~/p/g/c/drop-in  ➦ 2258a0f  git branch -a                                                                                                                                                                         Sun Mar 24 02:30:14 2024
* (HEAD detached at 2258a0f)
  feature/part-1
  feature/part-2
  feature/part-3
  main
 ~/p/g/c/drop-in  ➦ 2258a0f  git checkout main                                                                                                                                                                     Sun Mar 24 02:30:53 2024
Switched to branch 'main'
 ~/p/g/c/drop-in    ls                                                                                                                                                                                            Sun Mar 24 02:31:07 2024
flag.py
 ~/p/g/c/drop-in    cat flag.py                                                                                                                                                                                   Sun Mar 24 02:31:08 2024
print("Printing the flag...")
 ~/p/g/c/drop-in    git blame flag.py                                                                                                                                                                             Sun Mar 24 02:31:10 2024
^2258a0f (picoCTF 2024-03-12 00:07:54 +0000 1) print("Printing the flag...")
 ~/p/g/c/drop-in    git log                                                                                                                                                                                       Sun Mar 24 02:31:15 2024
commit 2258a0f267d57e8b6025e2a020b77fac7a553c92 (HEAD -> main)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:54 2024 +0000

    init flag printer
 ~/p/g/c/drop-in    git checkout feature/part-1                                                                                                                                                                   Sun Mar 24 02:31:18 2024
Switched to branch 'feature/part-1'
 ~/p/g/c/drop-in   feature/part-1  ls                                                                                                                                                                             Sun Mar 24 02:31:37 2024
flag.py
 ~/p/g/c/drop-in   feature/part-1  cat flag.py                                                                                                                                                                    Sun Mar 24 02:31:38 2024
print("Printing the flag...")
print("picoCTF{t3@mw0rk_", end='')⏎                                                                                                                                                                                                           ~/p/g/c/drop-in   feature/part-1  git checkout feature/part-2                                                                                                                                                    Sun Mar 24 02:31:40 2024
Switched to branch 'feature/part-2'
 ~/p/g/c/drop-in   feature/part-2  cat flag.py                                                                                                                                                                    Sun Mar 24 02:31:55 2024
print("Printing the flag...")

print("m@k3s_th3_dr3@m_", end='')⏎                                                                                                                                                                                                            ~/p/g/c/drop-in   feature/part-2  git checkout feature/part-3                                                                                                                                                    Sun Mar 24 02:31:57 2024
Switched to branch 'feature/part-3'
 ~/p/g/c/drop-in   feature/part-3  cat flag.py                                                                                                                                                                    Sun Mar 24 02:32:02 2024
print("Printing the flag...")

print("w0rk_6c06cec1}")
 ~/p/g/c/drop-in   feature/part-3    
 
 
 
 picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_6c06cec1}
 
--------------------------------------------------------------------------------------------------------------------------------------------------------


binhexa
 |  | 100 points
Tags: 
AUTHOR: NANA AMA ATOMBO-SACKEY

Description
How well can you perfom basic binary operations?
Start searching for the flag here nc titan.picoctf.net 49964


picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d6f8047e}


 !  ~/p/general_skills  nc titan.picoctf.net 49964                                                                                                                                                         27.7s  Sun Mar 24 02:42:02 2024

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10001011
Binary Number 2: 11111000


Question 1/6:
Operation 1: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 11111011
Correct!

Question 2/6:
Operation 2: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 10001000
Incorrect. Try again
Enter the binary result: 11101110000
Incorrect. Try again
Enter the binary result: 11101110000'

Incorrect input. Provide the right input
Enter the binary result: 11101110000
Incorrect. Try again
Enter the binary result: 01000011010101000
Correct!

Question 3/6:
Operation 3: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 000100010110
Correct!

Question 4/6:
Operation 4: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 0110000011
Correct!

Question 5/6:
Operation 5: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result:  10001000
Correct!

Question 6/6:
Operation 6: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 01111100
Correct!

Enter the results of the last operation in hexadecimal: 30 31 31 31 31 31 30 30

Incorrect input. Provide the right input!

Enter the results of the last operation in hexadecimal: 303131313131313030
Incorrect answer!

Enter the results of the last operation in hexadecimal: 7C

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d6f8047e}



------------------------------------------------------------------------------------------------------------------------------------------------------------------------






