# CSE 15L Week 1 Lab Report
In this tutorial, I will be describing how to log into a course-specific account on `ieng6`.
## First, install VScode
Go to the Visual Studio Code website and follow the websites instructions for installing it on your computer. After the application is installed, you should be able to open it to a page such as this:
![Image]  

Open a new terminal on VS Code. You can do this by hovering over the "Terminal" option in the upper bar, and selecting "New Terminal."

Then, type in the following command(replacing the provided email with your actual email):
```
ssh cs15lwi23abc@ieng6.ucsd.edu
```
SSH stands for secure shell, and allows two devices to communicate with one another.

You may then receive an output warning you of the host's authenticity. As this is a new server you are connecting to, it is reasonable to receive this message, and you should reply yes.
Then, your terminal should provide you with a password prompt. While you will not be able to visually see your password being typed, you should type in your password as normal.
If it is the correct password, your terminal should output the following message, indicating that you now have access to a computer in the lab from your personal device. The computer in the lab serves as the server, while your personal device serves as a client.

