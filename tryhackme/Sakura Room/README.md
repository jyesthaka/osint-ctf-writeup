# Sakura Room

Here's the write up for Sakura Room on TryHackMe.

## PART 1 - INTRODUCTION 

We'll skip this part

Answer: Let's Go!


## PART 2 - TIP-OFF

### Question: What username does the attacker go by?

Given an image that can be opened in the browser. The first instinct was to view page source of the image and there's this part:

<img width="854" height="427" alt="image" src="https://github.com/user-attachments/assets/5bf30529-6717-482e-b44e-ba1a5e70f62b" />

### Answer: SakuraSnowAngelAiko


## PART 3 - RECONNAISSANCE

### Question: What is the full email address used by the attacker?

To search for the email address: Google the username SakuraSnowAngelAiko and a Github page will show up. In their profile, there is a PGP repo with a public key than can be decrypted. Using this, an email was found:

<img width="1271" height="169" alt="image" src="https://github.com/user-attachments/assets/b3992e1f-d8a3-43b5-bb13-4df94e671456" />

### Answer: SakuraSnowAngel83@protonmail.com

### Question: What is the attacker's full real name?

By Googling SakuraSnowAngelAiko, there will also be a website that is pops up that shows this:

<img width="1164" height="216" alt="image" src="https://github.com/user-attachments/assets/46065c33-bdf8-4ab4-aab2-463c6b355a7c" />

This is clearly the user's real name

### Answer: Aiko Abe

## PART 4 - UNVEIL

### Qeustion: What cryptocurrency does the attacker own a cryptocurrency wallet for?

In the GitHub profile that the user owned which we have already seen, there is also a ETH repo (commonly ETH is Ethereum)

### Answer: Ethereum

### Question: What is the attacker's cryptocurrency wallet address?

In that specific repo, there is also a miningscript that contains a wallet: 0xa102397dbeeBeFD8cD2F73A89122fCdB53abB6ef

### Answer: 0xa102397dbeeBeFD8cD2F73A89122fCdB53abB6ef

### Question: What mining pool did the attacker receive payments from on January 23, 2021 UTC?

There is a website called etherscan.io where we can paste this and look at the activities done by the wallet owner

<img width="502" height="95" alt="image" src="https://github.com/user-attachments/assets/c144ab20-4024-4ec4-b84d-1e6d13bbc5d8" />

On January 23, 2021, there is 1 activity by this certain user and it is seen that he was receing from a mining pool called Ethermine

<img width="605" height="31" alt="image" src="https://github.com/user-attachments/assets/e3ec6810-4ffe-46a7-a872-0ec465b59a27" />

### Answer: Ethermine

### Question: What other cryptocurrency did the attacker exchange with using their cryptocurrency wallet?

We can simply just see that the user has exchanged in other forms of cryptocurrency which is Tether

<img width="615" height="93" alt="image" src="https://github.com/user-attachments/assets/e75306b0-7685-4b0b-a4c7-f98381247b76" />

### Answer: Tether

## PART 5 - TAUNT

### Question: What is the attacker's current Twitter handle?

In the beginning, we have found that the user has a new Twitter handle: SakuraLoverAiko

### Answer: SakuraLoverAiko

### Question: What is the BSSID for the attacker's Home WiFi?

We have to find BSSID and one of the webs that we can use is wigle.net

From the Twitter, the user shared about an AP and directed us to deep paste the AP (shown on the tweet):

<img width="713" height="205" alt="image" src="https://github.com/user-attachments/assets/416f91e6-21c2-44a8-9158-45c7799534aa" />

From here, we found that the SSID is DK1F-G and there is 1 result that shows up when it is inputted in wigle.net, which has a BSSID of 84:af:ec:34:fc:f8

### Answer: 84:af:ec:34:fc:f8

## PART 6 - HOMEBOUND

### Question: What airport is closest to the location the attacker shared a photo from prior to getting on their flight?

In the Twitter page, there is an image that the user uploaded, showing cherry blossom trees.

<img width="484" height="399" alt="image" src="https://github.com/user-attachments/assets/ed1d0a5e-bd13-49f4-96f0-f8a425904038" />

It is also said that the user is about to head home by flight. So we have to find the location of the image first. 

On the image, we can see that there is a monument in the back:

<img width="91" height="180" alt="image" src="https://github.com/user-attachments/assets/16e1941c-fe8e-4b66-b082-4024602173c8" />

Using Google Lens, we can see that there is an Instagram post that shows the monument, but is still unclear

<img width="224" height="363" alt="image" src="https://github.com/user-attachments/assets/d34b7985-d2fb-4ba5-8dc9-730db76d7c74" />

Using this image, I screen snipped it and used Google Lens again and found a match

<img width="208" height="423" alt="image" src="https://github.com/user-attachments/assets/1f401d1a-8df6-4593-9a31-75f9aa3ab0c6" />

It is shown that this monument is the Washington Monument where the nearest airport to this building is the Ronald Reagan Washington National Airport or DCA

### Answer: DCA

### Question: What airport did the attacker have their last layover in?

The user uploaded an image on his Twitter account about his last layover

<img width="309" height="321" alt="image" src="https://github.com/user-attachments/assets/531e65c4-8571-4e50-b536-61a06cddb571" />

Using Google Images where we input the text on the image, we can find the exact airport the user had their last layover at

<img width="437" height="354" alt="image" src="https://github.com/user-attachments/assets/e403406d-af8a-4438-9bb3-5aa6d84076c7" />

On the captions, it is stated that the airport is Haneda airport with the code HND 

### Answer: HND

### Question: What lake can be seen in the map shared by the attacker as they were on their final flight home?

There is a map showing a lake that was uploaded by the user on their Twitter account

<img width="486" height="317" alt="image" src="https://github.com/user-attachments/assets/1d22275f-34e7-4995-b075-0c659d7dcee3" />

Using Google Lens, I got a picture that looks similar to the one the user uploaded

<img width="361" height="307" alt="image" src="https://github.com/user-attachments/assets/bd5ece8f-7486-46bb-b7f2-8c72af89ad15" />

We can see this image and when looking into it again, it is Lake Inawashiro

<img width="321" height="294" alt="image" src="https://github.com/user-attachments/assets/5a09bc7a-81e2-47aa-8bdd-35d8b42f5394" />

### Answer: Lake Inawashiro

### Question: What city does the attacker likely consider "home"?

From the previous deep pasting, it is already discovered that the hometown is Hirosaki.

Therefore, CTF solved.
