---
layout: post
title:      "“What you seek is seeking you.” Rumi"
date:       2020-08-06 22:28:13 +0000
permalink:  what_you_seek_is_seeking_you_rumi
---


I started my first Flatiron School project with the above quote in mind, simply because it illustrates my attitude towards the big task that I had to face. I began the work on my program by thinking about the code I wish I had, writing pseudo code with test data, progressing to check if it works, and finally replacing it with the real time data gathered using an **API** call. I also tried to make my code as **DRY** as possible.  

**The Goal and  Purpose:**

The main goal of my project was partial utilization of the vast resources stored at Discogs.com website by the means of using **API** calls which, in return, would give the user of the program the ability to search information about artists and albums listed on the website and return valuable information about them.

**Functionality:**

The search functionality of the program is based on **Discogs API** and I used **Faraday gem** to obtain the information from it. The data that I initially received belonged to the string class and I had to parse it with **JSON**. This, in turn, converted the data into hash, making it much easier to work with. I wanted to use open uri, however this solution would not allow me to access all resources stored on Discogs.com due to the fact that Discogs API resources require authorization with customer key and customer secret, those attributes would have to be passed in headers and this is something that open uri could not handle.

 In order to make the reading of the **JSON** easier for myself I utilized a ruby library called **awesome print**, that was displaying the data on the terminal in full color making it simple to process.

**UX Personalization** 

In order to improve and personalize user experience I started the program with soliciting user names by using .**get.strip** method, so that once that is obtained, the program could greet its users by their own names and give them the option to search for the required information about a certain artist or an album that they like. The program itself has built-in input validation. It works by checking whether a user entered one of 3 available options and if wrong input is recorded, the user gets an error message. 

**Display of results**

Entering number 1 in the console, and typing the name of the artist, gives users the ability to access the information about a particular author, typing 2, on the other hand, displays the details of the album of their choice. Once the user is finished with his activity, he can type 3, in the terminal window, to close the program.

**Beautification**

Overall user experience was enhanced by the .colorize gem that added a pinch of esthetics to the program and made both the feedback soliciting and data display visually pleasing.

**Refactoring & Abstracting**

Once all methods in my project worked like a well-oiled machine, I proceeded to refactor my code by making it more abstract. This was done by grouping methods based on the functions that they performed for the project and adding them to their unique classes.


