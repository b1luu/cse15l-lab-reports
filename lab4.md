# Lab Report 4: Command Line Tasks:

## Timing Tasks: 

### 1. Setup:

Steps:
* Delete any existing forks to your repository regarding to [Lab 7](https://github.com/ucsd-cse15l-s23/lab7). If this doesn't show in your repository, please disregard this message. 

### 2. Setup Part 2:

Steps:
* Since [Lab 7](https://github.com/ucsd-cse15l-s23/lab7) isn't in your repository, you need to fork the repository [here](https://github.com/ucsd-cse15l-s23/lab7). 
* Forking [Lab 7](https://github.com/ucsd-cse15l-s23/lab7) is availble in the top-right of the screen, and press `Fork`.

## 3. The Real Deal: Set a Timer

Steps:
* Since we want to practice efficency in utilizing command line arguments, we are going to time our tasks as a way to measure progress and create a friendly environment that promotes improvement. 
* We can setup a timer via website, a good recommendation can be found [here](https://www.timeanddate.com/stopwatch/). Alternatively, we can use our phone's application as a mean to set a timer.

## 4. Log into ieng6

Steps:
* Either the choice of an IDE such as VSCode or direct terminal such as Command Prompt on Windows can access ieng6 login via terminal.
- To access the terminal on VSCode, you can download the IDE [here](https://code.visualstudio.com/download) + <enter> if you dont have the application downloaded and wish to use it as your terminal. 
>The expected website page to the link should be:

![Image](https://user-images.githubusercontent.com/120772535/231031750-f474c858-1f92-4ab4-b714-0ddf22bc6a24.png)
* Click the blue button, **Download for Windows**. If you are using a device that isn't windows, click the arrow (down arrow on the blue button) and download the platform specific to your device. 

>Once you have VSCode installed, begin to open the application. The screen page should look like this: 

![image](https://user-images.githubusercontent.com/120772535/231033020-5f5eee43-b4a7-441a-856a-34a598ea5a75.png)

Notice the top-left of VSCode, and click **Terminal** --> **New Terminal**. Notice you can also click `Control + Shift + ~ + <Enter>` as a command to create a new terminal. 

>Terminal should look like this at an area of your screen within VSCode:

![image](https://user-images.githubusercontent.com/120772535/231034075-0f01da24-bf92-41bd-99b1-e365696e2cb9.png)

* After having your terminal open, we want to type `shh cs15sp23XX@ieng6.ucsd.edu + <Enter>`. Notice: XX is only used for reference of this username format, each username is different and for that we advise you know your specific username in order to log into ieng6. 
  
>If you are having trouble locating your account; you can locate your CSE15L Account by clicking the link here: [Link](https://sdacs.ucsd.edu/~icc/index.php). Type in your UCSD username and Student ID. Once you are logged in, under section **Additional Accounts** you will find your CSE15L username and copy the username. 

  
  
Once you press <Enter>, you will get a prompt for you to type in your password. Your password should be the password you use to connect to UCSD's Webreg and myTritonLink you created upon enrolling. Please type it in and press <Enter>. 

*Be aware that typing feedback isn't shown while you are typing the password*

> Your screen should look like this:

![image](https://user-images.githubusercontent.com/120772535/231037278-12438fb9-f230-41c7-bbf9-358f4612decd.png)

  
* After typing your password, keypress <Enter>, and if done correctly, you are now logged into ieng6 and confirmation should look like this: 

![image](https://user-images.githubusercontent.com/120772535/231037467-e8551f71-3e2b-454a-b395-8d0dbb9c2df3.png)

## 5. Cloning repository from Github account
  
* In the terminal, type `git clone https://github.com/ucsd-cse15l-s23/lab7 + <Enter>`

![Screenshot 2023-05-22 200017](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/0cc965c1-88a6-4b90-883b-87678757634d)

  
## 6. Demonstrating Test Failure: 
* After cloning, we need to access to lab7 directory, you can do this by typing `cd lab7/ + <Enter>`

![Screenshot 2023-05-22 200536](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/2ff1e49e-e2f0-463e-af77-2d53eaa6982b)
  
* Use `pwd` to check that you are in the correct directory followed by pressing `<Enter>`. 
* After pressing `pwd`, in order to run the test, type `bash test.sh` in order to run the test ListExamples.java followed by `<Enter>`.
> Here is an image on what it should look like:
![image](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/a8a3c7a5-09dd-4849-9e31-04bfaaf05cfd)

  
## 7. Fix Code Failure:

* In order to fix the code, we need to access vim in order to edit the bug. Begin by typing `vim ListExamples.java`.
>The terminal should look like this:
![Screenshot 2023-05-22 204508](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/3727ddd2-ba83-43b0-9f92-198d8d393b16)

* When accessed to this screen, we are in vim's normal mode, which doesn't allow direct typing editing access. In order to do so, we need to press `<I>` to switch to insert mode, an alternative, editing access mode.
* The error can be access by going downward in line #36, we need to do this by using the `<J>` keystroke, which is used in vim to go down a single line. We need to press this 36 times. In addition, you can use arrow keys while in insert mode, go you can use `<right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><right-arrow-key><backspace><2>`.
* To exit, we need to press `<escape>` and then followed by `<:wq!>`.
![Screenshot 2023-05-22 204824](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/fb856bb0-82d2-442c-862d-a328e964abd8)


## 8. Demonstrating Code Success:

* In reference to the [Lab 7](https://github.com/ucsd-cse15l-s23/lab7) website, highlight the compiler in order to run the test, `<Control-C><Control-V>' on 'javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` followed by `<Enter>`. This will compile ExamplesListTests.java and create a class file.
*Then `<Control-C><Control-V>' on `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ...` followed by `<Enter>`.
>On the bottom of the command after running `ListExamples.java`, instead of the failure message, it should pop up 2 tests passing.
![IMG_9348](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/1aacf533-2418-456d-83a4-c193aef18c9b)

## 9. Commit and Push

*After the test has worked and have passed, you will need to commit and push the edited file to Github. In order to do so, we need to type the command `git add ListExamples.java` followed by `<Enter>`. 
*Next, we need to commit the file by typing `git commit -m "(any message you like)"` followed by `<Enter>`.
*Finally, we need to push it back to Github by typing `Git push` followed by `<Enter>`. 
>The terminal you are accessing should look like this: 
![Screenshot 2023-05-22 211158](https://github.com/b1luu/cse15l-lab-reports/assets/120772535/61836265-76a1-4c2b-9030-0909a4c067f6)




