# CSE 15L Lab Report 4
## CSE Labs "Done Quick"
In this lab, we attempted to complete routine tasks using shortcuts in order to maximize efficiency. 

The steps for the tasks were numbered and given to us. The first step is to delete any existing forks of the lab7 repository. This can be done by going into the fork's settings, scrolling down and selecting "Delete this repository." The second step is to fork the repository. The third step before we get into the lab is to start the timer!

### Step 4: Log into ieng6
*Keys pressed: ```<up><enter>```*

The *```ssh cs15lwi23adu@ieng6.ucsd.edu```* command was 1 up in the search history, so I used the up arrow to access it. Thanks to our pre-lab set-up of setting up ssh keys in GitHub, I no longer have to type my password in as I am authenicated using a private key file on my local machine. 

<img width="963" alt="Screen Shot 2023-02-27 at 11 29 50 AM" src="https://user-images.githubusercontent.com/122496338/221663813-5b2bad7f-c4d3-4002-841f-cd54fa40356a.png">

### Step 5: Clone Your Fork of the Lab7 Repository

To clone the repository, I copied the SSH key found in my GitHub fork: 

<img width="417" alt="Screen Shot 2023-02-27 at 11 33 13 AM" src="https://user-images.githubusercontent.com/122496338/221664480-95e514dd-3afe-4a53-8a9e-018476ff25cb.png">

Then, I typed out the command ```git clone git@github.com:anushaprao/lab7.git``` and pressed ```<enter>```.
<img width="963" alt="Screen Shot 2023-02-27 at 11 36 25 AM" src="https://user-images.githubusercontent.com/122496338/221665134-e54d0568-535d-4fc5-8348-9a415cdb2de7.png">

### Step 6: Running the Tests to Demonstrate Errors in the Code
The first thing I must make sure I do is change into the lab7 directory in order to access the files in that directory.
<img width="1005" alt="Screen Shot 2023-02-27 at 4 33 14 PM" src="https://user-images.githubusercontent.com/122496338/221721257-9009f204-ad94-4595-a2af-02e40e4f7de8.png">

*Keys pressed: ```<up><up><up><up><up><up><up><up><up><enter>```*

The *```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java```* command was 9 up in my search history, so I used the up arrow to access it instead of typing out the command. 
<img width="979" alt="Screen Shot 2023-02-27 at 4 48 01 PM" src="https://user-images.githubusercontent.com/122496338/221723137-57060f19-2818-4c07-a720-f97e54b47a4c.png">


*Keys pressed: ```<up><up><up><up><up><up><up><up><up><enter>```*
The *```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests```* command was 9 up in my search history, so I used the up arrow to access it instead of typing out the command. 
<img width="1010" alt="Screen Shot 2023-02-27 at 4 47 20 PM" src="https://user-images.githubusercontent.com/122496338/221723048-f19da701-2509-4d98-b6e9-448f9137b367.png">
After running the tests, we can see that 2 of the tests ran, and that 1 of them failed, indicating an error in the code.

### Step 7: Editing the Code to Fix the Failing Test
I typed out the command ```nano ListExamples.java``` and pressed ```<enter>```.
<img width="973" alt="Screen Shot 2023-02-27 at 4 56 23 PM" src="https://user-images.githubusercontent.com/122496338/221724314-2c80c166-d0b7-40bb-8500-c5c12dc724f6.png">

The nano command opens this window:
<img width="1008" alt="Screen Shot 2023-02-27 at 4 56 37 PM" src="https://user-images.githubusercontent.com/122496338/221724324-cde19037-8161-4018-b528-f53e7ba66fdb.png">

I scrolled down the file until I reached the line that I noticed the error on.
*Keys pressed: ```<right><right><right><right><right><right><right><right><right><right><right><right><2><right><right><delete>```*
These keystrokes helped me reach the location of the error (the code was incrementing index1 instead of index2) and helped me rectify the issue.

After fixing the file, I needed to save the file and exit nano.
*Keys pressed: ```<ctrl-o><enter><ctrl-x>```*
This set of keystrokes will save the file(ctrl-o) and then exit nano(ctrl-x), returning the user to the terminal.

### Step 8: Re-running the Tests to Demonstrate Success
*Keys pressed: ```<up><up><up><enter>```*
The *```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java```* command was 3 up in my search history, so I used the up arrow to access it instead of typing out the command. 
<img width="1000" alt="Screen Shot 2023-02-27 at 5 03 26 PM" src="https://user-images.githubusercontent.com/122496338/221725321-3cdcff8f-cafb-4493-b169-6bcacb234d93.png">

*Keys pressed: ```<up><up><up><enter>```*
The *```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests```* command was 3 up in my search history, so I used the up arrow to access it instead of typing out the command.
<img width="999" alt="Screen Shot 2023-02-27 at 5 14 46 PM" src="https://user-images.githubusercontent.com/122496338/221726926-abd66bc1-4f00-4d1a-843d-f867a2b7b6a8.png">
This command demonstrates that both the tests have passed, and that we have rectified the issue with the initial code.

### Step 9: Commit and Push to GitHub Account
During the lab, my groupmates and I experimented with add, commit and push commands and discovered that we could combine all of these commands into one line. So, in order to add, commit, and push the changes in the code to my GitHub account, I typed out the command ```git commit -am "Updated" && git push``` and pressed ```<enter>```.
<img width="1013" alt="Screen Shot 2023-02-27 at 5 18 27 PM" src="https://user-images.githubusercontent.com/122496338/221727488-e589fc6a-b805-4d5f-bf35-e671b5720718.png">

To double check that our file was updated, we can go to our lab7 fork on the GitHub website, and we can double check that ListExamples.java is updated, which we can see through the commit message "Updated". 
<img width="1440" alt="Screen Shot 2023-02-27 at 5 22 48 PM" src="https://user-images.githubusercontent.com/122496338/221728185-4c1d198d-c1df-4aa6-a9f9-ef8b17bad4ff.png">
We can also verify the updates by selecting the ListExamples.java file and double-checking that the error in the original code was corrected:
<img width="338" alt="Screen Shot 2023-02-27 at 5 25 00 PM" src="https://user-images.githubusercontent.com/122496338/221728506-d2caf35c-2aa1-49a9-8f1a-82b6c4b5ede1.png">


