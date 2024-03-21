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
 
 
 

