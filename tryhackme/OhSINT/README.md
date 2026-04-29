## Challenge Info

**Title:** OhSINT  
**Category:** OSINT  
**Difficulty:** Easy  
**Description:**  
This challenge involves gathering information about a user using various OSINT techniques across multiple platforms.

## Solution

Honestly I don't feel satisfied with this one because I had to look up some ways to get the answer

**What is this user's avatar of?**

Before I began, I downloaded the file attached to the challenge which is a file of the Windows wallpaper. To gather more information, I used an exiftool online to gather some information

<img width="815" height="55" alt="image" src="https://github.com/user-attachments/assets/6bbd79e7-52ca-4274-a379-7a9a113dfdd8" />

Turns out that this file belongs to OWoodFlint and when I search that username online, I found a Twitter page.

<img width="601" height="331" alt="image" src="https://github.com/user-attachments/assets/f6be9143-18ae-45f4-b87d-db94d54fe91b" />

This Twitter page's profile picture is a cat

Answer: cat

**What city is this person in?**

When searching the username OWoodFlint, there is also a GitHub page and it shows the city the person is in

<img width="937" height="616" alt="image" src="https://github.com/user-attachments/assets/456a04e5-6a75-4ccb-8d3d-f929834b24b1" />

Answer: London

**What is the SSID of the WAP he connected to?**

On the Twitter page, this person tweeted this:

<img width="590" height="127" alt="image" src="https://github.com/user-attachments/assets/bac7e570-7b0f-4a3f-8a3f-a49e1e8f3e18" />

I used wigle.net to look deeper into this. Using their view feature and entering the BSSID and zooming out the map, there is (I think) a satellite coming from the UK which matches where this person is from and it shows that the SSID is UnileverWiFI

<img width="196" height="106" alt="image" src="https://github.com/user-attachments/assets/94815f9e-0075-4549-92fc-8c2428bc2264" />

Answer: UnileverWiFi

**What is his personal email address?**

This was also in the user's GitHub page

Answer: OWoodflint@gmail.com

**What site did you find his email address on?**

Pretty self explanatory. Found it on GitHub.

Answer: GitHub

**Where has he gone on holiday?**

The user attached a wordpress link on his GitHub that shows where the user is right now

<img width="736" height="144" alt="image" src="https://github.com/user-attachments/assets/f2f1ef18-b19a-47a0-a82a-53965ecc5beb" />

Answer: New York

**What is the person's password?**

Looking at the wordpress source code, it is shown that the user's password is pennYDr0pper.!

Answer: pennYDr0pper.!

CTF Solved. Although this might really be a low point for me because I really had a lot of help doing this from the internet. Hopefully I don't have to do things like that again.

## Flag

N/A

## Comment

Beginner-friendly OSINT challenge that covers multiple techniques such as metadata analysis, username pivoting, WiFi intelligence, and basic web source inspection.
