# Description

This time Network Security Sam remembered to upload the password file, but there were deeper problems than that.

# Solution

Remember when I said to learn `F12` source code view?

Now we are using it again.

Sam uploaded the psw file this time.

But he made a major mistake.

So open sorce code `F12` and use `inspect element` click inside the psw input field.

Within the `HTML5` code you can see a line whic says the following.

`<input type="hidden" name="file" value="password.php">`

This is basically a hidden file wich is only visible here.

but it gives us the password file too.

To access it just enter into the URL

after the general URL string hackthissite.org/missions/basic/3`/password.php`

and hit enter.

A new page will load in containing the password.

Which is `1e0154d2`

Off you go to level 4