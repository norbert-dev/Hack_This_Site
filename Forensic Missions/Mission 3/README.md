 Mission 3::
        
        	Title:: Papa Smurphey's Pizza
            Brief:: Examine copied files for evidence.
            Difficulty:: Medium

Mission description (detailed)::

	The local police just arrested a suspect believed to be the notorious "PapaSmurphey", 
    an online pizza trader. Any violation of the federal pizza law is a serious crime, 
    and convicted offenders face severe statutory penalties. For example, a first time 
    offender convicted of producing pizza under 18 U.S.J. 2251 faces fines and a statutory 
    minimum of 15 years to 30 years maximum in prison. A flash drive was recovered from 
    the scene and was copied; poorly. As best as you can, examine the contents for 
    any incriminating evidence on the suspect.

*This challenge has several steps. 
The completion password will look like this: HTS{the_answer}*

How do we start?
	
Honestly I dont know. 

I am gonna write my entire thought method here now. 

The first thing popping up is that the ssh.jpg is actualy a WHOLE lot bigger than the other jpgs. 

So it has to do something with the solution. 
I am also thinking about that every other file except siggies.txt is just a decoy.

I am thinking about this one because the ssh.jpg properties say this is a 500 * 500 jpg file with a dpi of 100px so this must contain other elements as well. Especialy if we compare the file sizes with the other jpgs. 

Could be this big but I do feel it has to do with the solution.

I have run spectrum analisys on the audio file nothing there also tried to change its extension for some might be hidden stuff but nothing there as well. So lets just consider this as well as a dummy file too.
    
This reduces us with 2 files only.

    siggies.txt
    and
    shh.jpg

Ok now we are moving. 

So lets open up the ssh.jpg in a hex viewer. 

Luckily https://hexed.it/ is more than enough for this purpose. 
Now let's see the siggies.txt as well. 

What do we know about jpgs? 

They always have a given header wich is followed by a given trailer.

Here on headers and trailers come into play siggies.txt. 
    
Example every jpg image starts with a header HEX: [ FF D8 ] and trails with [ FF D9 ]. 
Everything in between this two HEX info is the picture. 

Now if we check the ssh.jpg HEX code we can see that after the trailer there are more data. 
This suggest more thing to look for. 

Now there are offsets what we need to encounter.

To do that we contribute and thank Nick Duely for a python code. See attached.

Lets run this code.
    
After runing the code we have extracted 2 rar files and 3 images.

0.rar is psw protected 1.rar is corrupted this is the offset data.

2.jpg is the original cover image of ssh.jpg 3.jpg is corruted offset data and 4.jpg says 
    "GL0zMe" 
this might be the code to unzip 0.rar.

Lets try it. Wow it works.!!!

So now we extract all files from 0.rar.

There are a bunch of them but one stands out. In particular the 

    "DNM Login.txt"

Let's open it up. 
And here is the flag.

    HTS{You_caught_me!}