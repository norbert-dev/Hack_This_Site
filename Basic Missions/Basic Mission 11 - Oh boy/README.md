# Description

Sam decided to make a music site. Unfortunately he does not understand Apache. This mission is a bit harder than the other basics.

# Solution

Now this is I believe one of those missions which gets every each one of us by knowledge. 

Not that easy.

Whenever you refresh the page a random music appears.

Lets try `F12` and `Inspect tool`

Not much here except a tipp.
But this appears on every songs page.

`<!--We even have our own collection - if you could find it!-->`

Ok this is something. Lets take this forward. Lets step back to the original site. 

I was not paying too much attention to them but Oh boy I should have. One thing is common in all of the music appearing.

They are songs from `Elton John`

Now since there are no files shown! No new info! No whatever only one thing I could think after a long while are `folder`

Now in apache all folders are listed in URL. A folder call is enabled if you close the call functon with a `/`.

Do some research on how to hide folders in apache. I suggest you do it too. Comes handy here.

So lets try random abc folders folder `a/`, `b/`, `c/` etc if you know what I mean.

By the songs I was going with the folder `elton/` but gave me an ERROR.

Next I tried `john/`

Same Error.

Then I went all nuts and enterd `e/` and wow.

`https://www.hackthissite.org/missions/basic/11/e/` folder exists.

so I went down this rabbit hole untill this point.

`https://www.hackthissite.org/missions/basic/11/e/l/t/o/n/`

Here my research payed off. You can hide files and folders with the `.htaccess` file.

Lets add this to our folder structure.
Because in general this is a hidden file. So it makes sence that we cant see it.

`https://www.hackthissite.org/missions/basic/11/e/l/t/o/n/.htaccess`

And here we are.

The file says.

`IndexIgnore DaAnswer.* .htaccess
<Files .htaccess>
require all granted
</Files>`

This file basicaly tells the server what to show and not to show. Also this is a dangerous file. Do your research and you will understand why.

So it says `IndexIgnore Da Answer.* .htaccess`

Ok lets see the answer file or folder.

If we add this to our folder structure

`https://www.hackthissite.org/missions/basic/11/e/l/t/o/n/DaAnswer`

We get this message.

`The answer is not here! Just look a little harder.`

OK now I was sitting over this a LONG LONG WHILE. Then it got obvious.

Tear this sentence appart.

The ANSWER IS `not here`

This is the password. I have to mention that the answer always changin here but the theory is the same for the pwd.

Ok but where do I enter this now.

Well the page you are looking at is not the real or original `index.html`

lets add index.html to the URL string.

We will end up at the same page. So one more thing left try index.php.

`https://www.hackthissite.org/missions/basic/11/index.php`

And there you go. Enter the password of yours and you are done with the basic missions.

# PS

This last mission is a really hard one. I personaly spent about a week to do it and think about it also researching it. And I honestly learnt a lot of it too.

I can HIGHLY suggest to you to do the same. This way you will understand it far better.







