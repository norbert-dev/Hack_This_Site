# Description

Network Security Sam has encrypted his password. The encryption system is publically available and can be accessed with this form:

You have recovered his encrypted password. It is:

`14g8h:?l`

	ps:: the last char in the code is a small L

Decrypt the password and enter it below to advance to the next level.

# Solution

Now this is something. This is actually challanging and we have to think.

So at first I had to things in my mind.

1. Bruteforce the hell out of it! 

Ok but how? No infos we got on reversing the code. So Lets stick to my second option.

2. Try and error random

First trying all letters numbers would take a long time randomly.

So let us see what we get if we enter just 1 `a` into the form. We might can get a patern. 

The answer is `a = a`

so now lets add a few more a's to it.

Lets make it 5 a's that should give some result.

By entering 5 a's we get `aaaaa = abcde` do you see the patern?

Let me do one last thing and I'll explain after lets see we have an encrypted 8 digit psw. So lets enter 8 a's and I can tell thet it will give me back this.

`aaaaaaaa = abcdefgh`

CHECH IT if you doubt me but this is the result.

So we have a patern the first digit doesnt change the 2nd skips 1 char the 3rd skipps 2 etc. So for the 8 digits it will be

`0 +1 +2 +3 +4 +5 +6 +7` 

for the skipped letters. Now we can easily assign a number value to the encrypted digits just look up the ASCII codes by ASCII the encryped code looks like this 

` 049 052 103 056 104 058 063 049`

Now all we have to do is reversing the code so instead of + we deduct the amounts from the ASCII numbers. Use ASCII code chart that helps a lot here.

`0 -1 -2 -3 -4 -5 -6 -7`

Then we get this 

`049 051 101 053 100 053 057 101`

So the final code will be is u numareta this will be 

password: `13e5d59e`

And now you are good to go.



