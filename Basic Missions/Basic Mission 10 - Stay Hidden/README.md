# Description

Please enter a password to gain access to level 10

# Solution

Well lets see. Enter whatever into the psw input field.

Lets say `abc123`

AHHHHH you did not think this will work right? But it actualy did.

The message you get is this.

`You are not authorized to view this page`

So this means that we have to gain authority over it.

Kind a simple let me explain lets go back to the previous page first.

So authority is managed by cookies. We can use 3rd party apps and softwares to capture cookies but we can speed things up by knowing JavaScript.

Lets insert a few JavaScript code.

Open up `F12` Sorce code view and you can see next to inspect elements the following `Elements, Console, Sources etc..`

Select `Console`

Enter the following injection code.

`javascript:alert(document.cookie);`

then hit enter.

You will see a pop up window appear saying a few things. Like this.

`level10_authorized=no; PHPSESSID=ou7sa2ojs76u7ffh7l3pe7bog0; HackThisSite=makimebgndvni4f9cvo0igjh13; style_cookie=null; __htsCookieNotice=1`

There we are at the very first statement. We have NO authority to pass. Lets change that.

Enter the next javascript inject code.

`javascript:void(document.cookie="level10_authorized=yes"); `

And hit enter now we have authority.

We can procced to level 11 even with an empty password input field. But if you want you can enter whatever.

Lets see the last level.