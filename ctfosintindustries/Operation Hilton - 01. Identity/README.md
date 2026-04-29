## Challenge Info

**Title:** Operation Hilton — 01 · Identity  
**Category:** OSINT  
**Points:** 5  
**Description:**  
BRIEFING
20:36 ET. Washington Hilton, Connecticut Avenue NW. The annual White House Correspondents' Dinner is in full swing when the evacuation is triggered. Five to eight gunshots reported in the immediate vicinity of the perimeter. President Trump is extracted by the Secret Service. A suspect is apprehended on site.

You're the OSINT analyst on duty. The FBI has shared two photos of the seized equipment on social media. The press has only released a name and an age. It's up to you to reconstruct the file.

Authorized sources: tweets @tacticalporn, @ippatel, Secret Service · MPDC · NBC · CBS · Reuters · AP · BBC press releases.

Flag format: OSINT{...} — case sensitive, exact format required.

TASK
The suspect was identified by the DC Metropolitan Police Department.

Provide his full name, age, and hometown.

## Solution

This challenge was pretty straightforward and easy. I had to find the full name of the shooter, his age, and his hometown.

The challenge was provided with very useful sources such as this Tweet:

<img width="626" height="755" alt="05f51e63-00ac-4b2a-a65f-d795d3cb51a4" src="https://github.com/user-attachments/assets/3af8aef5-1b70-45f4-b1b3-b9519ec7d03b" />

This tweet shows 60% of the flag which is his full name: Cole Thomas Allen (which wasn't exactly right)

Next step I did was look his name up on Google.

LA Times posted an article regarding the incident and it turns out his name was actually Cole Tomas (without the H) Allen. Just from the headline, it shows that he was from Torrance. 

Next step is to find his age. In another article published by NBC News:

<img width="628" height="129" alt="image" src="https://github.com/user-attachments/assets/f974e074-4ec0-4f82-8f6a-7f4eb9aebb8e" />

It shows that he is 31. 

## Flag

OSINT{Cole_Tomas_Allen_**_********}

✔ Identity correlation performed  
✔ Data triangulated from multiple sources  
✔ Output validated successfully

## Comment

CTF Solved. Wasn't really that hard though. I hope the next one is just slightly tougher.
