Mission 1::
        
        	Title:: First Time Go
            Brief:: Recover the deleted password file.
            Difficulty:: Easy
            
Mission description (detailed)::

	From: stacy.melroy@tritech.org

	Thank you for agreeing to help me. We recently had a problem with a former employee and though I cannot prove it, I believe he is the one that erased the files off my thumbdrive. I did some research and I made an image of the drive for you but that is as far as I got. I can replace most of what was lost but there is one file in particular that holds a very important account password. If you could recover that file, I would be extremely grateful.

	Also, this is my personal thumbdrive. Keep that in mind please. I'm not sure what you might recover, but I would rather it not get spread around.

	-Attachment here-
	md5checksum: 4e7af965caed9b8d29c40f549fdb7d28
    
How do we get started?

First as always read the mission carefully because in most cases it does give you hints where to go.
In our case for now we can only download the given recovery file attachment.
Lets do it so.
After downloading this we will have a image.tar.gz compressed file.
    
This can be extracted with pretty much anything. We need to do this twice to access the given recovery image.
this is gona be << image.dd >>.
    
Now as always we hit a wall here. Whats a "dd" file?? 
Lets do what a good IT shaq person would do and lets ask google.
    
Google says that a *.dd file is a disk image file and replica of a hard disk drive.
    
Thats more than enough to know for now. So we know its a disk image which is like *.iso etc. So we need a tool to attach it to our system. Lets use google again.
    
I personaly used OSF Mount this can handle *.dd files. After attaching the image.dd as a HDD in OSF we obtain the saved HDD under the name of 'stacy'. This contains a main folder and subfolders
    .Trash-1000 
        - expunged
        - files
        - info
    
All folders empty. So when we get a step closer we do also get a step back. Almost like standing still. Lets think for a second where are we now. We received the zip file which got unzipped. We successfully mounted the *.dd HDD iso file to our system. But the files got trashed so we have to recover the files which were deleted by the employee.

Check.

How do we do it.? Ok if you are not certain but I know that you know what to do.
    
YES
    
Google
    
Lets look for "recovery tool for deleted files" I am sure that you will come across 

Recuva.

Here you can download it if needed::
https://www.ccleaner.com/recuva/download

Fine download / Install / Run.
Straigh forward and here it goes. Recuva found 22 files which can be restored. Lets save them into a folder.
There is a restored file called "Your new password is.rar" but this si psw protected. Lets dig in what we have.
There are many pictures and pdfs but there is a Voice Mail from the tech support. The tech guy tells Stacy to use her number for the new password.
Lets find her number. After opening the files we got we can find a Termination word doc file. This has Stacys number 519-555-4783 
The psw is the numbers so 5195554783 no dashes.
No we can open the "Your new password is.rar" file and the doc file inside.
And here we are the solution password is there.
    
    Password is:: qPYgbs0w5&?i{8a