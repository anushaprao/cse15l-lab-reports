# CSE 15L Week 1 Lab Report
In this tutorial, I will be describing how to log into a course-specific account on `ieng6`.
## First, install VScode
Go to the Visual Studio Code website and follow the website's instructions for installing the application on your computer. I already had VSCode downloaded on my computer, so I was able to skip this initial step. After the application is installed, you should be able to open it to a page such as this:
<img width="1026" alt="Screen Shot 2023-01-11 at 4 29 21 PM" src="https://user-images.githubusercontent.com/122496338/212778422-a46598a5-cb08-4566-bfc6-194b2befe299.png">

## Next, let's try remotely connecting to a server
Open a new terminal on VS Code. You can do this by hovering over the "Terminal" option in the upper bar, and selecting "New Terminal."

Then, type in the following command(replacing the provided email with your actual email):
```
ssh cs15lwi23abc@ieng6.ucsd.edu
```
SSH stands for secure shell, and allows two devices to communicate with one another.

You may then receive an output warning you of the host's authenticity. As this is a new server you are connecting to, it is reasonable to receive this message, and you should reply yes.
<img width="851" alt="Screen Shot 2023-01-16 at 3 24 41 PM" src="https://user-images.githubusercontent.com/122496338/212779500-96815255-128a-4d87-8fee-9d6b1f5eabf7.png">

Then, your terminal should provide you with a password prompt. While you will not be able to visually see your password being typed, you should type in your password as normal.
If it is the correct password, your terminal should output the following message, indicating that you now have access to a computer in the lab from your personal device.
<img width="1173" alt="Screen Shot 2023-01-16 at 3 23 29 PM" src="https://user-images.githubusercontent.com/122496338/212779401-1fbca0a0-cc71-42f0-8205-1a4177dcf133.png">
The computer in the lab serves as the **server**, while your personal device serves as a **client**.

## Trying some commands
Now, we can try to input some commands into our terminal. The command
```
ls -lat
```
displays a list of file and directory names. 
Similarly,
```
ls -a
```
also outputs a list of all file and directory names.
<img width="916" alt="Screen Shot 2023-01-16 at 3 26 48 PM" src="https://user-images.githubusercontent.com/122496338/212779784-b8fe4ee0-2d2f-4c8a-8258-6466e431af94.png">

The command
```
cd
```
followed by a directory name will allow you to change directories.

The command
```
cd ~
```
can be used to change the current directory back to the original home directory.

The command
```
mkdir
```
can be used to create a new directory, when the command is followed by a inputed name.
<img width="379" alt="Screen Shot 2023-01-16 at 3 50 41 PM" src="https://user-images.githubusercontent.com/122496338/212781559-d3fd7345-ac5e-4d67-880b-eb691527dfc9.png">


The command
```
pwd
```
displays the full path name of the user's current directory, starting at the root directory.

<img width="368" alt="Screen Shot 2023-01-16 at 3 48 57 PM" src="https://user-images.githubusercontent.com/122496338/212781418-f3847f63-0d04-449a-9907-f1088a31fb0b.png">

The command
```
cp
```
can be used to copy the contents of one file into another file.

Hopefully, this tutorial helps you install VSCode, connect remotely, and try some commands in your terminal.


