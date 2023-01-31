# CSE 15L Week 2 Lab Report
## Part 1- StringServer
I used the NumberServer.java file from the Week 2 Lab as the basis for my StringServer code, refining different parts to better fit the prompt. 
Here is the code for my StringServer:
<img width="1011" alt="Screen Shot 2023-01-30 at 4 36 54 PM" src="https://user-images.githubusercontent.com/122496338/215628698-06e82ee7-d587-4795-acd8-9b2293572174.png">
<img width="932" alt="Screen Shot 2023-01-30 at 4 37 24 PM" src="https://user-images.githubusercontent.com/122496338/215628714-2ba18ef1-fe7a-42ad-a1de-e5b44f9cb022.png">

The method called in my code is handleRequest.Starting with an empty string and an empty String ArrayList, the conditional checks if the path is simply a "/", in which case it returns a list containing all the strings added to the web server. If the path contains "/add-message," the string following the "=" sign in the query is added to the list and displayed on a new line. If the URI url provided is not the correct one, a "404 Not Found" error is returned. In addition, the class StringServer ensures that any port the web server is called to be hosted on is a valid port number. If it is not a valid port, or a port is not present, the user is prompted to request another port number. 

Example 1 using /add-message:
<img width="1439" alt="Screen Shot 2023-01-30 at 6 41 35 PM" src="https://user-images.githubusercontent.com/122496338/215649210-36ec7b66-41b7-43b3-ac92-2e0f5643f976.png">
<img width="1440" alt="Screen Shot 2023-01-30 at 4 55 48 PM" src="https://user-images.githubusercontent.com/122496338/215631747-d37e24d3-1b2a-4226-84a9-72e62a7d7a6d.png">

Example 2 using /add-message:

<img width="1440" alt="Screen Shot 2023-01-30 at 4 57 28 PM" src="https://user-images.githubusercontent.com/122496338/215631943-2cda64d1-1344-4061-b022-0559101482f2.png">
<img width="1440" alt="Screen Shot 2023-01-30 at 4 57 52 PM" src="https://user-images.githubusercontent.com/122496338/215631954-2447352a-d016-42cd-97c4-b1983c9d992e.png">

In both these examples, the method called in my code is handleRequest. The relevant arguments to these methods are a URI url whose path the conditional statement within the method parses to check the query. The values entered into this field in the first example is the string "Hello," and the value for the second example is the string "Goodbye." The value of the ArrayList list is updated when the method is called.

## Part 2- Bugs from Lab 3
The bug from Lab 3 that I have chosen to explore is the bug in the averageWithoutLowest function found in the ArrayExamples.java file. The function's intended purpose is to take the average of all the numbers in an array, except the lowest number, and return the mean. If there are no elements or only one element in the array, a 0 is returned. 
Here is the before code for the averageWithoutLowest function prior to any debugging:
```
static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  }

```

A failure-inducing input for this function can be seen through the following JUnit test:
```
@Test
  public void testlowest() {
    double[] input1 = {1,2,3,4,5,1};
    assertEquals(3.0, ArrayExamples.averageWithoutLowest(input1), 1e-9);
  }
```
<img width="806" alt="Screen Shot 2023-01-30 at 6 17 57 PM" src="https://user-images.githubusercontent.com/122496338/215643260-cd4ad3b3-27cf-44e0-a925-7f9e11ebcf28.png">
The expected output is 3.0, found by solving (2+3+4+5+1)/5. While 1 is the lowest value in the array, we only want to remove one instance of the lowest number, not all instances. The output for this test is the incorrect value of 2.8. 


A correct output for this buggy function can be seen through the following JUnit test:
```
@Test
  public void testlowest() {
    double[] input1 = {1,2,3,4,5};
    assertEquals(3.5, ArrayExamples.averageWithoutLowest(input1), 1e-9);
  }
```
<img width="855" alt="Screen Shot 2023-01-30 at 6 22 42 PM" src="https://user-images.githubusercontent.com/122496338/215644205-758cd009-e986-4dad-9793-bc769f542308.png">
The expected output is 3.5, found by solving (2+3+4+5)/4. 1 is the lowest value in the array, and as there is only one instance of this value, the mean is properly calculated. The output for this test is the correct value of 3.5, which does not indicate any need for debugging.   

#### Fixing the Bug:
The bug that needed to be fixed is that currently the program accounts for and removes all instances of the lowest number, failing to allow other instances of the smallest number(save for the first instance)to be accounted for in the mean. In order to solve this bug, I included a count variable which is initialized to 0. Upon the loop's first encounter with the lowest number, the count will be incremented to 1. As long as count is greater than 1(meaning the lowest variable has already been accounted for) or the number is not lowest(necessary to account for the first instance of the lowest number), the value at that index of the array will be added to the sum total in order to find the mean.
The correct code block is:
```
static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) {
         lowest = num; }
    }
    double sum = 0;
    int count = 0;
    for(double num: arr) {
      if (num == lowest){
        count += 1;
      }
      if(count > 1 || num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  }
```

Re-running this code for the first JUnit test now produces the correct value of 3.0, as can be seen by the output of the test.
<img width="854" alt="Screen Shot 2023-01-30 at 6 34 36 PM" src="https://user-images.githubusercontent.com/122496338/215648012-fec0fd48-5cb7-4440-ab94-6d482460d6c9.png">


## Part 3- Something New I Learned from Lab 2 or Lab 3
In week 2 and week 3, I learned a lot of new material which was fascinating to me. Looking at Week 2's lab, the information learned about ports was very interesting to me. In particular, with learning how to host a server on a remote computer. As there are only 3 ieng6 computers, there are only 3 port 4000 available to host the server on. Learning how to then utilize another port to deploy a web server was a challenge for my lab partner and I. Exploring the code and deploying it proved to be an interesting learning experiment and taught me a lot about how to host and deploy servers.
