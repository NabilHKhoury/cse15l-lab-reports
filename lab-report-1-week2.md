# Week 2 Lab report
## Tutorial for Lab 1
Hi, my name is Nabil. I am a student in CSE 15L. I have learned some software techniques that have made logging into a course-specific account. This is necessary for this course, and also I would think it isnecessary for having an industry job where one may need to code. Therefore, I will make this tutorial of how I did it in the circumstance that I need to relearn how to do this, or in the circumstance someone takes CSE 15L and needs help completing this process. 
### Step 1: Installing VScode
Although I already have VScode downloaded on my computer, and therefore, do not need to rememeber how to do this. Therefore, I will link a great youtube video on how to do this incase someone needs to download and learn the basics of this IDE. Press this [Link](https://www.youtube.com/watch?v=VqCgcpAypFQ). 

![Image](Screenshot (38).png)
### Step 2: Remotely Connecting
To remotely connect to a course-specific account, the first step is to install [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse). Then in the terminal of VScode, type ssh then the course specific email. A promot will ask for a password and we must type it in. If we have done this correctly the data of the accounf will be displayed in the terminal. 

![Image](Screenshot (39).png)
### Step 3: Run Some Commands
Once were in the account, we can run some command from the user end of the course-specific account. Some examples of commands that one can run is ls, which lists the files in the directory, or pwd, which prints the current working directory, or mkdir, which makes a new directory that we can name after typing in mkdir. 
![Image](Screenshot (40) edited.png)

### Step 4: Moving Files with scp Command
If we have a file that is already created on our desktop that we want to add to our course-specific account, we can use the command scp then file name then course loggin followed by :~/. This will prompt the users password, and after entering the password the filer will be moved into the home directory
![Image](Screenshot (41).png)

### Step 5: SSH Keys
If you have gotten to this point, you must know that it is annoying to have to type in a password every time you log into the account. Having a file on our computer with a key will allow us to not have to do this and will grant us automatoc access to the account once we type in the email. To do this, we need to type in the command ssh-keygen, which will generate a public and private key. it will prompt for a paraphrase, which you should not do just click enter to skip. It will then save the public key and spit out a random image that will work as the key to logging in. We then need to copy the public key to the .ssh directory of the user account server. Now, we will not need a password to loggin or do any of the functionalities that require a password. 

![Image](Screenshot (43).png)
![Image](Screenshot (44).png)

### Step 6: Optomizing Remote Running
Since we spent so much time setting up the keys so we would not need to have to enter a password, we now cna optomally move files with scp as we did earlier. We can use a different file and try the same thing and do the process in one command. Once we are in the account, we can also use ls command as mentioned to show this process worked and that our hard work has paid off.
 
![Image](Screenshot (45).png)
