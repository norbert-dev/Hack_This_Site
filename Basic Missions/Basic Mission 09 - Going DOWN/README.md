# Description

Network Security Sam is going down with the ship - he's determined to keep obscuring the password file, no matter how many times people manage to recover it. This time the file is saved in /var/www/hackthissite.org/html/missions/basic/9/.

In the last level, however, in my attempt to limit people to using server side includes to display the directory listing to level 8 only, I have mistakenly screwed up somewhere.. there is a way to get the obscured level 9 password. See if you can figure out how...

This level seems a lot trickier then it actually is, and it helps to have an understanding of how the script validates the user's input. The script finds the first occurance of '<--', and looks to see what follows directly after it.

# Solution

As always READ FIRST and understand.

This part is important

"In the last level, however, in my attempt to limit people to using server side includes to display the directory listing to level 8 only, I have mistakenly screwed up somewhere.. there is a way to get the obscured level 9 password."

So we can get access to level 9 password @ level 8.

Lets go back to level 8.

`https://www.hackthissite.org/missions/basic/8/`

As we learned at level 8 SSI UNIX command `<!--#exec cmd="ls ../"-->`

we only need to update the command a little. Like this.

`<!--#exec cmd="ls ../../9"-->`

This will give us the following

`Hi, index.php p91e283zc3.php! Your name contains 24 characters.`

Guess what. Open the `p91e283zc3.php` file as we already know how. BUT this time not under mission 8 URL but mission 9s.

Like this `https://www.hackthissite.org/missions/basic/9/p91e283zc3.php`

And there we are.

Our password is: `faa0492f`

And we are good to go.

keep it up not much left here. Lets see level 10

