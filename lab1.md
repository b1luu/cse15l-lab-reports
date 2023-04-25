# Lab Report 1: 

## How to Install Visual Studio Code

*Vistual Studio Code, commonly VSCode, is an IDE that allows for editing code-based text for the purpose of developing, testing, debugging code which will unfold into various programs.*

How to install VSCode:

Step 1: Make sure you have access to the internet, and visit the website link [here](https://code.visualstudio.com/). 

>The expected website page to the link should be:

![Image](https://user-images.githubusercontent.com/120772535/231031750-f474c858-1f92-4ab4-b714-0ddf22bc6a24.png)

***

Step 2: Click the blue button, **Download for Windows**. If you are using a device that isn't windows, click the arrow (down arrow on the blue button) and download the platform specific to your device. 


>Once you have VSCode installed, begin to open the application. The screen page should look like this: 

![image](https://user-images.githubusercontent.com/120772535/231033020-5f5eee43-b4a7-441a-856a-34a598ea5a75.png)
***

## How to Connect Remotely 

Step 1: Notice the top-left of VSCode, and click **Terminal** --> **New Terminal**. Notice you can also click `Control + Shift + ~` as a command to create a new terminal. 

>Terminal should look like this at an area of your screen within VSCode:

![image](https://user-images.githubusercontent.com/120772535/231034075-0f01da24-bf92-41bd-99b1-e365696e2cb9.png)



Step 2: Locate Your CSE15L Account by clicking the link here: [Link](https://sdacs.ucsd.edu/~icc/index.php). Type in your UCSD username and Student ID. Once you are logged in, under section **Additional Accounts** you will find your CSE15L username and copy the username. 


Step 3: Type in the terminal and write ` ssh [Username (paste what you copied previously here)] ` + ` @ieng6.ucsd.edu ` followed by pressing **Enter**
> Your command should look similar to this: 
Code: ` ssh cs15lsp23zz@ieng6.ucsd.edu ` where zz is used to create a general instance. 

![image](https://user-images.githubusercontent.com/120772535/231036552-914fa7c5-4eb1-42dc-b0e1-c583de489cec.png)

*If you are logging in for the first, type `yes` followed by **Enter***

Step 3: Once you press *Enter**, you will get a prompt for you to type in your password. Your password should be the password you use to connect to UCSD's Webreg and myTritonLink you created upon enrolling. Please type it in and press **Enter**. 

*Be aware that typing feedback isn't shown while you are typing the password*

> Your screen should look like this:

![image](https://user-images.githubusercontent.com/120772535/231037278-12438fb9-f230-41c7-bbf9-358f4612decd.png)


Step 4: Congratulations! You are connected to remotely and your Terminal should look like this:

![image](https://user-images.githubusercontent.com/120772535/231037467-e8551f71-3e2b-454a-b395-8d0dbb9c2df3.png)

## Running Some Commands

Step 1: Notice command-lines such as `ls`, `cd`, `~`, `ls <directory> `, and `cat /home/linux/ieng6/cs15lsp23/public/hello.txt`. 

Step 2: Try running those commmands within the terminal: 
> After running the commands, your terminal should look like this: 

![image](https://user-images.githubusercontent.com/120772535/231038431-f13f4892-a633-4e78-bd7b-90f90b621c64.png)


## Conclusion:

You can begin to test around and try various combination of commands, once you are complete with running the commands, the server will close once you exit out of VSCode. Upon relogging, you will need to re-enter your password. 



***




