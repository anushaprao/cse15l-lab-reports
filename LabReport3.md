# CSE 15L Lab Report 3
## Researching Commands
The command I selected for this lab report was *grep*. 

The first command line option that I utilized was -c. This option returns the number of lines that match the string/pattern that is being searched for. 

**Example 1:**
Running the code:
```
grep -c "air-conditioning" written_2/travel_guides/berlitz1/*.txt
```
results in
```
written_2/travel_guides/berlitz1/HandRHawaii.txt:2
written_2/travel_guides/berlitz1/HandRHongKong.txt:1
written_2/travel_guides/berlitz1/HandRIbiza.txt:0
written_2/travel_guides/berlitz1/HandRIsrael.txt:2
written_2/travel_guides/berlitz1/HandRIstanbul.txt:0
written_2/travel_guides/berlitz1/HandRJamaica.txt:3
written_2/travel_guides/berlitz1/HandRJerusalem.txt:0
written_2/travel_guides/berlitz1/HandRLakeDistrict.txt:0
written_2/travel_guides/berlitz1/HandRLasVegas.txt:0
written_2/travel_guides/berlitz1/HandRLisbon.txt:0
written_2/travel_guides/berlitz1/HandRLosAngeles.txt:1
written_2/travel_guides/berlitz1/HandRMadeira.txt:0
written_2/travel_guides/berlitz1/HandRMadrid.txt:0
written_2/travel_guides/berlitz1/HandRMallorca.txt:0
written_2/travel_guides/berlitz1/HistoryDublin.txt:0
written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:0
written_2/travel_guides/berlitz1/HistoryEgypt.txt:0
written_2/travel_guides/berlitz1/HistoryFWI.txt:0
written_2/travel_guides/berlitz1/HistoryFrance.txt:0
written_2/travel_guides/berlitz1/HistoryGreek.txt:0
written_2/travel_guides/berlitz1/HistoryHawaii.txt:0
written_2/travel_guides/berlitz1/HistoryHongKong.txt:0
written_2/travel_guides/berlitz1/HistoryIbiza.txt:0
written_2/travel_guides/berlitz1/HistoryIndia.txt:0
written_2/travel_guides/berlitz1/HistoryIsrael.txt:0
written_2/travel_guides/berlitz1/HistoryIstanbul.txt:0
written_2/travel_guides/berlitz1/HistoryItaly.txt:0
written_2/travel_guides/berlitz1/HistoryJamaica.txt:0
written_2/travel_guides/berlitz1/HistoryJapan.txt:0
written_2/travel_guides/berlitz1/HistoryJerusalem.txt:0
written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt:0
written_2/travel_guides/berlitz1/HistoryLasVegas.txt:0
written_2/travel_guides/berlitz1/HistoryMadeira.txt:0
written_2/travel_guides/berlitz1/HistoryMadrid.txt:0
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:0
written_2/travel_guides/berlitz1/HistoryMallorca.txt:0
written_2/travel_guides/berlitz1/IntroDublin.txt:0
written_2/travel_guides/berlitz1/IntroEdinburgh.txt:0
written_2/travel_guides/berlitz1/IntroEgypt.txt:0
written_2/travel_guides/berlitz1/IntroFWI.txt:0
written_2/travel_guides/berlitz1/IntroFrance.txt:0
written_2/travel_guides/berlitz1/IntroGreek.txt:0
written_2/travel_guides/berlitz1/IntroHongKong.txt:0
written_2/travel_guides/berlitz1/IntroIbiza.txt:0
written_2/travel_guides/berlitz1/IntroIndia.txt:0
written_2/travel_guides/berlitz1/IntroIsrael.txt:0
written_2/travel_guides/berlitz1/IntroIstanbul.txt:0
written_2/travel_guides/berlitz1/IntroItaly.txt:0
written_2/travel_guides/berlitz1/IntroJamaica.txt:0
written_2/travel_guides/berlitz1/IntroJapan.txt:0
written_2/travel_guides/berlitz1/IntroJerusalem.txt:0
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:0
written_2/travel_guides/berlitz1/IntroLasVegas.txt:0
written_2/travel_guides/berlitz1/IntroLosAngeles.txt:0
written_2/travel_guides/berlitz1/IntroMadeira.txt:0
written_2/travel_guides/berlitz1/IntroMadrid.txt:0
written_2/travel_guides/berlitz1/IntroMalaysia.txt:0
written_2/travel_guides/berlitz1/IntroMallorca.txt:0
written_2/travel_guides/berlitz1/JungleMalaysia.txt:0
written_2/travel_guides/berlitz1/WhatToDublin.txt:0
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:0
written_2/travel_guides/berlitz1/WhatToEgypt.txt:0
written_2/travel_guides/berlitz1/WhatToFWI.txt:0
written_2/travel_guides/berlitz1/WhatToFrance.txt:0
written_2/travel_guides/berlitz1/WhatToGreek.txt:0
written_2/travel_guides/berlitz1/WhatToHawaii.txt:0
written_2/travel_guides/berlitz1/WhatToHongKong.txt:0
written_2/travel_guides/berlitz1/WhatToIbiza.txt:0
written_2/travel_guides/berlitz1/WhatToIndia.txt:0
written_2/travel_guides/berlitz1/WhatToIsrael.txt:0
written_2/travel_guides/berlitz1/WhatToIstanbul.txt:0
written_2/travel_guides/berlitz1/WhatToItaly.txt:0
written_2/travel_guides/berlitz1/WhatToJamaica.txt:0
written_2/travel_guides/berlitz1/WhatToJapan.txt:0
written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:0
written_2/travel_guides/berlitz1/WhatToLasVegas.txt:0
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:0
written_2/travel_guides/berlitz1/WhatToMadeira.txt:0
written_2/travel_guides/berlitz1/WhatToMalaysia.txt:0
written_2/travel_guides/berlitz1/WhatToMallorca.txt:0
written_2/travel_guides/berlitz1/WhereToDublin.txt:0
written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:0
written_2/travel_guides/berlitz1/WhereToEgypt.txt:0
written_2/travel_guides/berlitz1/WhereToFWI.txt:0
written_2/travel_guides/berlitz1/WhereToFrance.txt:1
written_2/travel_guides/berlitz1/WhereToGreek.txt:0
written_2/travel_guides/berlitz1/WhereToHawaii.txt:0
written_2/travel_guides/berlitz1/WhereToHongKong.txt:0
written_2/travel_guides/berlitz1/WhereToIbiza.txt:0
written_2/travel_guides/berlitz1/WhereToIndia.txt:0
written_2/travel_guides/berlitz1/WhereToIsrael.txt:0
written_2/travel_guides/berlitz1/WhereToIstanbul.txt:0
written_2/travel_guides/berlitz1/WhereToItaly.txt:0
written_2/travel_guides/berlitz1/WhereToJapan.txt:0
written_2/travel_guides/berlitz1/WhereToJerusalem.txt:0
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:0
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:0
written_2/travel_guides/berlitz1/WhereToMadeira.txt:0
written_2/travel_guides/berlitz1/WhereToMadrid.txt:0
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:2
written_2/travel_guides/berlitz1/WhereToMallorca.txt:0
```
This code is going through each file in this directory and searching for the word "air-conditioning" and returning how many instances of that word occur in each file. This can be useful information for someone searching for travel destinations with specific key-term amenities in mind.

**Example 2:**
Running the code:
```
grep -c "Orange County" written_2/travel_guides/berlitz1/HandRLosAngeles.txt
```
results in:
```
1
```
The -c command can also be used on individual files to have the number of instances of a search word returned. If a user is curious about a certain appearing in a specific text, they can search and see how many times it is mentioned. 

I found this command line option at [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/). 

---

The second command line option that I looked at was -n. This option returns the line number and the line that the string/substring being searched for is found on within a given file.

**Example 1:**
Running the code:
```
grep -n "Orange County" written_2/travel_guides/berlitz1/HandRLosAngeles.txt
```
results in:
```
9:        area and Orange County. All hotels are of a high standard, with private
```
Similar to the -c command, the -n command goes through all the lines in a given file and returns the line which the search word is found on.

**Example 2:**
Running the code:
```
grep -n "air-conditioning" written_2/travel_guides/berlitz1/*.txt
```
results in:
```
written_2/travel_guides/berlitz1/HandRHawaii.txt:109:        kitchens and ceiling fans (no air-conditioning, TVs, or phones). The
written_2/travel_guides/berlitz1/HandRHawaii.txt:232:        outdoor enthusiasts. Rooms are quaint, with no air-conditioning.
written_2/travel_guides/berlitz1/HandRHongKong.txt:9:        Hotels listed below have full air-conditioning, offer 24-hour or
written_2/travel_guides/berlitz1/HandRIsrael.txt:93:        air-conditioning and TV in the rooms) is situated very close to the
written_2/travel_guides/berlitz1/HandRIsrael.txt:177:        cabins come with kitchen, bathroom, and air-conditioning, are set on
written_2/travel_guides/berlitz1/HandRJamaica.txt:49:        modern, with tiled floors and air-conditioning. 23 rooms. Major credit
written_2/travel_guides/berlitz1/HandRJamaica.txt:127:        with air-conditioning (some with loft) and cable TV. 25 rooms. Major
written_2/travel_guides/berlitz1/HandRJamaica.txt:204:        swinging hammocks. All rooms have air-conditioning and ceiling fan.
written_2/travel_guides/berlitz1/HandRLosAngeles.txt:10:        bath, air-conditioning, television, and telephone; most have king- or
written_2/travel_guides/berlitz1/WhereToFrance.txt:756:        the water pipes, blue for the air-conditioning ducts, and yellow for
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:377:        in the days before air-conditioning. These havens of relaxation set
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:2445:        orchids. Highly efficient air-conditioning makes life tolerable for
```
The -n command also works with searching for a key term throughout each file in a directory, and lists the line and file where the word being searched for is found in each file. This is useful for instances when a certain key term is being searched for as it allows the user to see where specifically in the file the term can be found. This is useful for larger files as the user does not have to absently search the returned file for the keyword and rather can target the specific line.

I found this command line option at (https://www.geeksforgeeks.org/grep-command-in-unixlinux/).

---

The third command line option that I experimented with was -i. This option returns all lines that contain the string being searched for with no delineation based on case. Meaning it searches for both upper- and lower-case variations of the string being searched for.

**Example 1:**
Running the code:
```
grep -i "orange county" written_2/travel_guides/berlitz1/HandRLosAngeles.txt
```
results in:
```
area and Orange County. All hotels are of a high standard, with private
```
Although the term being searched for (orange county) is not capitalized, the -i command searches for any variation of the search word, and finds the capitalized words within the file.

**Example 2:**
Running the code:
```
grep -i "san pedro" written_2/travel_guides/berlitz1/*.txt
```
results in:
```
written_2/travel_guides/berlitz1/HistoryLasVegas.txt:        In 1903, officials of the San Pedro, Los Angeles, and Salt
written_2/travel_guides/berlitz1/IntroLasVegas.txt:        railroad officials from the San Pedro, Los Angeles, and Salt Lake
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:        Rey, San Pedro, or the Balboa Peninsula. For a more romantic outing,
written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:        San Pedro, Newport Beach, and several other points.
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        Palos Verdes to San Pedro
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        Amidst a bevy of beach towns is gritty San Pedro, a
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        for longer stays. It is easily reached byferry from San Pedro or Long
```
The -i command uses the grep command to search for the term "san pedro" and finds all instances of the term, presenting a list of the files which contain any instance of the searched word. The result is a list of files which contain San Pedro.

I found this command line argument at (https://www.softwaretestinghelp.com/grep-command-in-unix/).

---

The fourth command line option that I explored was -v. This option returns all the lines in a file which do not contain the key term being searched for. It is often referred to as an inverse command.

**Example 1**
Running the code:
```
grep -v "hotels" written_2/travel_guides/berlitz1/HandRLosAngeles.txt
```
results in:
```
Recommended Hotels
        price categories, grouped according to regions within the Los Angeles
        bath, air-conditioning, television, and telephone; most have king- or
        except on executive floors and at some budget motels that offer morning
        coffee, orange juice, and doughnuts or muffins.
        To make direct reservations with a hotel, we have included
        addresses (all in California, abbreviated CA) and telephone/fax
        numbers. Check-out time is generally noon or 1pm, with check-in usually
        Rates vary greatly according to season and availability;
        promotions. Ask about such discounts when booking. We have used the
        following symbols to indicate room prices (two persons in a double
        room, per night):
        ❁❁❁$200 and up
        ❁❁$100–$200
        ❁under $100
```
This result eliminates all the lines in the text file which contain the word "hotels." When I compared the file to this output, I observed that if a line contained the case-specific word "hotels," the output had eliminated the entire line when it printed. 

**Example 2**
Running the code:
```
grep -v "Las Vegas" written_2/travel_guides/berlitz1/HandRLasVegas.txt
```
results in:
```
Recommended Hotels
        By the year 2000, there were roughly 130,000 rooms in Las
        Vegas. This makes selecting a hotel room intimidating, but not
        impossible. One must consider the usual factors — cost, location, and
        budget — as well as how integral you want your hotel to be to your
        never leave your hotel premises.
        hotels in four price categories. For a comprehensive listing of
        Authority (see Accommodations on page 109).
        All businesses must comply with the Americans with
        Disabilities Act, and are therefore wheelchair accessible. Newer
        properties are the easiest to navigate, older and Downtown properties
        slightly more difficult.
        Mastercard, American Express). Price ranges listed do not include
        suites. Expect holiday and weekend rates to be significantly higher,
        and be sure to ask for specific quotes for your intended stay. For more
        information about most of these hotels, particularly with regard to
        their casinos and attractions, look in Where To Go starting on page
        26.
        $$$$over $200
        $$$$100–$200
        $$$50–$100
        $under $50
```
I thought that this output was very interesting to me as I was looking to eliminate any lines containing the phrase "Las Vegas." As the word is split over two lines at the start of the file, the -v command does not eliminate it from the text, demonstrating how it only searches to see if the term is contained within the line. An instance where the -v command could be useful is if the user had a list of names, and they were looking to see all the names beside a known one. 

I found this command line option at (https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/).
