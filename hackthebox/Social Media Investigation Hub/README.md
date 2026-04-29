## Challenge Info

**Title:** Social Media Investigation Hub  
**Category:** OSINT  
**Difficulty:** Very Easy  
**Description:**  
You've discovered Alex Morgan is connected to RivalTech and has been conducting fake review campaigns against TechFlow. Now you need to map Alex's complete digital footprint across social media platforms to understand the full scope of this operation and find evidence of coordination with other actors.

## Solution

Given 9 questions and I assume I have to answer all of the questions to get the flag

**Question 1: What is the real name of the person behind the TechReviewer2024 account across all platforms?**

Went to the ConnectPro page and found his real name

<img width="688" height="270" alt="image" src="https://github.com/user-attachments/assets/bbbb72d3-717f-45d9-a9a0-09bba6a8ae12" />

**Answer: Alex Morgan**

**Question 2: Which company did Alex Morgan previously work for according to their professional background?**

In this challenge, ChirpNet = Twitter, ConnectPro = LinkedIn, and ForumHub (I assume) is Reddit and to find someone's professional and academic background, always go to LinkedIn (in this case, ConnectPro)

<img width="683" height="684" alt="image" src="https://github.com/user-attachments/assets/0a9c8fa9-2bba-4192-88aa-5b3a457c6bd0" />

Previously he worked at RivalTech as a Marketing Specialist

**Answer: RivalTech Inc.**

**Question 3: What is the operation codename mentioned in the ForumHub coordination post?**

I don't really use Reddit that often as it was banned from my country so it was pretty confusing to get the context of the app

The only thing that helped me answer this one is the weird looking text format in one of the Reddit posts

<img width="593" height="251" alt="image" src="https://github.com/user-attachments/assets/3d0dadee-425b-4fa5-b703-6d0ced3f194a" />

**Answer: operation_social_storm_2024**

**Question 4: In which month and year were most of the suspicious reviewer accounts created?**

The ChirpNet following list shows that most suspicious accounts (@ReviewMaster_Bob, @TechTruth_Sally) were followed since February 2024, indicating coordinated account creation.

**Answer: February 2024**

**Question 5: What product is being specifically targeted in the negative review campaign?**

This person is publicly criticizing a product on his Reddit account which is the XyloPhone Pro

<img width="557" height="207" alt="image" src="https://github.com/user-attachments/assets/ca89acea-d6d6-461e-a20e-f2b432bf4f81" />

**Answer: XyloPhone Pro**

**Question 6: What role does TechReviewer2024 have in the TechReviews subreddit on ForumHub?**

<img width="653" height="129" alt="image" src="https://github.com/user-attachments/assets/8e91877f-0147-447c-b41f-a8aeffc49322" />

Here is shown his role as a moderator.

**Answer: moderator**

**Question 7: What is Alex Morgan's educational background according to ConnectPro?**

Exact method like when I figured out where he was last employed.

<img width="692" height="474" alt="image" src="https://github.com/user-attachments/assets/9c6d9e58-41c0-4a8b-b3b6-f129e04b6eb4" />

**Answer: University of California, Berkeley**

**Question 8: How many connections does Alex Morgan have on ConnectPro?**

Pretty straightforward.

<img width="679" height="273" alt="image" src="https://github.com/user-attachments/assets/83f71123-ab4f-499e-ac12-a0985fb0d802" />

**Answer: 89**

**Question 9: What is the total post karma that u/TechReviewer2024 has accumulated on ForumHub?**

Pretty straightforward as well.

<img width="335" height="101" alt="image" src="https://github.com/user-attachments/assets/9c3ee052-2aa6-44fd-a894-abbe94c32f2e" />

**Answer: 1247**

CTF Solved. Flag found.

## Flag

HTB{alexmorgan_operationsocialstorm2024_********}

✔ Social media footprint analyzed  
✔ Relevant activity identified  
✔ Findings validated

## Comment

Very easy OSINT challenge. Mostly straightforward platform mapping and basic information gathering.
