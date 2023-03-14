# CSE 15L Lab Report 5
## Looking Further at Lab Report 3: Researching Commands

One of my favorite lab reports we did was Lab Report 3, where I looked at 3 command line options for the *grep* command. I really enjoyed this lab because it showed me what I could practically use this command for, and it challenged me to implement it in my own terminal.
For Lab Report 5, I would like to take inspiration from the prompt and do a similar exploration for the *less* command. 

The first command line option that I utilized was utilizing less followed by a file path. This option returns the text file found at the file path location.

**Example 1:**
Running the code: 
``` 
less travel_guides/berlitz1/HandRLosAngeles.txt 
```
results in
```
Recommended Hotels
        The following hotels are listed alphabetically in three
        price categories, grouped according to regions within the Los Angeles
        area and Orange County. All hotels are of a high standard, with private
        bath, air-conditioning, television, and telephone; most have king- or
        queen-sized beds. Breakfast is not usually included at US hotels,
        except on executive floors and at some budget motels that offer morning
        coffee, orange juice, and doughnuts or muffins.
        To make direct reservations with a hotel, we have included
        addresses (all in California, abbreviated CA) and telephone/fax
        numbers. Check-out time is generally noon or 1pm, with check-in usually
        available from 2pm to 3pm. All hotels accept major credit cards.
        Rates vary greatly according to season and availability;
        many hotels offer special weekend packages, business rates, and
        promotions. Ask about such discounts when booking. We have used the
        following symbols to indicate room prices (two persons in a double
        room, per night):
        ❁❁❁$200 and up
        ❁❁$100–$200
        ❁under $100
```
This code is accessing the file found at the file path location and printing out the output of the content. This can be useful information for someone who knows the file name, but needs to find the contents of the file. Through tracing the results of the file path, they can find the content contained in the file on the server or device.

**Example 2:**
Running the code:
```
less travel_guides/berlitz1/HandRIbiza.txt   
```
results in
```
Recommended Hotels
        The establishments listed below offer a cross-section of
        local restaurants, and should convince you that not everything on the
        island comes with chips (french fries).
        The star rating in brackets after each entry refers to the
        offfical government rating system.
        As a basic guide, the symbols we use indicate what you can
        expect to pay for a three-course meal for two, excluding wine, tax and
        tip. Drinks will add considerably to the final bill.
        ✪less than 5,000 ptas.
        ✪✪5,000–8,000 ptas.
        ✪✪✪more than 8,000 ptas.
```
This code is going through through the filepath input for "HandRIbiza.txt" file and returns the file's content. This can be useful information for someone who knows they have a file and its path, but want to find out what's in the file.

I found this command line option at [https://phoenixnap.com/kb/less-command-in-linux](https://phoenixnap.com/kb/less-command-in-linux).

---

The second command line option that I utilized was -name. This option returns the file path that matches the file being searched for.

**Example 1:**
Running the code: 
``` 
less -N travel_guides/berlitz1/HandRIbiza.txt   
```
results in:
```
      1 
      2   
      3   
      4     
      5       
      6         Recommended Hotels
      7         The establishments listed below offer a cross-section of
      8         local restaurants, and should convince you that not everything on the
      9         island comes with chips (french fries).
     10         The star rating in brackets after each entry refers to the
     11         offfical government rating system.
     12         As a basic guide, the symbols we use indicate what you can
     13         expect to pay for a three-course meal for two, excluding wine, tax and
     14         tip. Drinks will add considerably to the final bill.
     15         ✪less than 5,000 ptas.
     16         ✪✪5,000–8,000 ptas.
     17         ✪✪✪more than 8,000 ptas.
     18       
     19     
     20   
```
This code operates very similar to the first less command, as it takes in a file path for a file, and returns a numbered output of the file's contents. This can be useful as some of these files do not begin at line 1, so if the user is looking for a file line that contains a certain phrase or term, they should utilize the correct line number as a reference.

**Example 2:**
Running the code: 
``` 
less -N travel_guides/berlitz1/HandRLosAngeles.txt   
```
results in:
```
      1
      2
      3
      4
      5
      6         Recommended Hotels
      7         The following hotels are listed alphabetically in three
      8         price categories, grouped according to regions within the Los Angeles
      9         area and Orange County. All hotels are of a high standard, with private
     10         bath, air-conditioning, television, and telephone; most have king- or
     11         queen-sized beds. Breakfast is not usually included at US hotels,
     12         except on executive floors and at some budget motels that offer morning
     13         coffee, orange juice, and doughnuts or muffins.
     14         To make direct reservations with a hotel, we have included
     15         addresses (all in California, abbreviated CA) and telephone/fax
     16         numbers. Check-out time is generally noon or 1pm, with check-in usually
     17         available from 2pm to 3pm. All hotels accept major credit cards.
     18         Rates vary greatly according to season and availability;
     19         many hotels offer special weekend packages, business rates, and
     20         promotions. Ask about such discounts when booking. We have used the
     21         following symbols to indicate room prices (two persons in a double
     22         room, per night):
     23         ❁❁❁$200 and up
     24         ❁❁$100–$200
     25         ❁under $100
     26
     27
     28
```
This code operates very similar to the first less command, as it takes in a file path for a file, and returns a numbered output of the file's contents. This can be useful as some of these files do not begin at line 1, so if the user is looking for a file line that contains a certain phrase or term, they should utilize the correct line number as a reference.

I found this command line option at [https://phoenixnap.com/kb/less-command-in-linux](https://phoenixnap.com/kb/less-command-in-linux).

---
The third command line option that I utilized was -p. This option highlights the term searched for after the letter p in the file.

**Example 1:**
Running the code: 
```
less -pHotels travel_guides/berlitz1/HandRLosAngeles.txt 
```
results in:

<img width="827" alt="Screen Shot 2023-03-13 at 9 41 14 PM" src="https://user-images.githubusercontent.com/122496338/224895246-151e06ef-782e-4b75-bce7-007193f992c6.png">

This code operates very similar to the second less command, with the user typing in the word they are searching for after the -p. In the above example, the search word is Hotels, and this term is highlighted in the output. This can be useful if a user is searching a file for a specific word and they would like to see the file output along with a search word. 

**Example 2:**
Running the code: 
```
less -photels travel_guides/berlitz1/HandRLosAngeles.txt 
```
results in:
<img width="769" alt="Screen Shot 2023-03-13 at 9 50 34 PM" src="https://user-images.githubusercontent.com/122496338/224896351-f2adcb3d-8db3-41dd-aa16-ab33fe531cb0.png">

Similar to the last example, the search word was hotels, but this time it was lower-case, demonstrating that the search is case-specific. This can be useful if a user is searching for a case-specific term.

I found this command line option at [https://phoenixnap.com/kb/less-command-in-linux](https://phoenixnap.com/kb/less-command-in-linux).





