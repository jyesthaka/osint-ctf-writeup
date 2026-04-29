## Challenge Info

**Title:** The Suspicious Domain  
**Category:** OSINT  
**Difficulty:** Very Easy  
**Description:**  
Following the discovery of the suspicious social media profile "TechReviewer2024", investigators have uncovered a review manipulation campaign targeting TechFlow. The domain "alexmorgan-reviews.net" appears to be central to this operation. Use DomainScope to investigate this domain and identify the key identifier linking it to the broader campaign infrastructure.

:: Challenge Type :: Interactive Q&A Platform (6 questions + 3 correlation questions).

:: How to Play :: (1) Click "Start Instance" and wait for the Docker container to spawn | (2) Open the given URL in your browser - this will take you to "DomainScope" | (3) The domain "alexmorgan-reviews.net" will be pre-loaded | (4) Explore the different tabs (WHOIS, DNS Records, Hosting, etc.) to gather intelligence | (5) Go to the "Investigation Challenge" tab (rightmost tab) | (6) Answer 6 questions about the domain | (7) Once you've answered all 6, you'll unlock the "Correlation Challenge" | (8) Finish the 3 extra correlation questions - the final flag will then show up on the page.
## Solution

Still on the very easy stage of HTB OSINT.

**Question 1: What is the registrant's email address from the WHOIS record?**

Here is the WHOIS:

<img width="454" height="902" alt="image" src="https://github.com/user-attachments/assets/d3ebae1a-54bf-4fd1-bad1-ab6c3f6df614" />

It is stated that the registrant contact is Alex Morgan

**Answer: Alex Morgan**

**Question 2: What is the complete phone number including country code?**

Still on the WHOIS

**Answer: +1-408-555-0987**

**Question 3: When was the domain created? (Format: YYYY-MM-DD)**

Still on the WHOIS (Creation Date: 2024-01-20)

**Answer: 2024-01-20**

**Question 4: What is the exact organization name from WHOIS?**

Still on the WHOIS (Organization: Morgan Tech Reviews LLC)

**Answer: Morgan Tech Reviews LLC**

**Question 5: What city is listed in the registrant's address?**

Still on the WHOIS (Registrant Contact -> City: San Jose)

**Answer: San Jose**

**Question 6: What is the domain's transfer status?**

This one is a little harder as I had to look up examples of transfer statuses.

It is still on the WHOIS (Domain Status: clientTransferProhibited)

**Answer: clientTransferProhibited**

**Question 7: What company is being targeted?**

From the hosting details:

<img width="1547" height="525" alt="image" src="https://github.com/user-attachments/assets/8868d4f0-8d31-4e37-91d7-b8c8390a15c0" />

The Digital Fingerprint shows the Google Analytics ID

**Answer: TechFlow**

**Question 8: What email service is the threat actor using?**

The threat analysis shows the information about the potential attack.

<img width="1535" height="441" alt="image" src="https://github.com/user-attachments/assets/eb6cd4f5-fa3a-411c-a4a7-1defa6345d40" />

**Answer: tempmail**

**Question 9: How many GitHub Pages IPs are configured?**

The DNS records shows 4 A records with 4 GitHub pages

<img width="1531" height="490" alt="image" src="https://github.com/user-attachments/assets/ec3ff44c-5822-45e5-8928-5ab3541d9ccc" />

**Answer: 4**

CTF Solved. Flag captured.

## Flag

HTB{alexmorgantempmailcom_********_********}

✔ Domain investigation conducted  
✔ WHOIS / infrastructure data analyzed  
✔ Output validated

## Comment

Very easy challenge focused on basic WHOIS analysis, DNS records, and simple threat intelligence correlation.
