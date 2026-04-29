## Challenge Info

**Title:** Find the Masked Man  
**Category:** OSINT  
**Difficulty:** Easy  
**Description:**  
This challenge involved analyzing an image to identify a hidden location and determine a nearby station. The flag format is `OSINT{STATION_NAME}`.

## Solution

The challenge started with an image containing a masked man. The first useful clue came from the background, where the word **“Julien”** was visible.

<img width="1536" height="2048" alt="mask" src="https://github.com/user-attachments/assets/62871f6d-135e-4f87-bff8-778df19e8483" />

Since the hint suggested a location near Paris, I searched for *“Julien Paris”* and found a matching place called **Maison Julien**.

<img width="941" height="721" alt="image" src="https://github.com/user-attachments/assets/3ec7b713-8d61-4350-ab7d-9ac9544028f2" />

To confirm the location, I compared the reference image with the real-world location using Google Images/Maps, which showed a strong match.

After identifying Maison Julien, I moved to Google Maps and searched for nearby stations in the area. The closest relevant station near the location was:

<img width="825" height="400" alt="image" src="https://github.com/user-attachments/assets/eb3d624b-b2fd-42f4-89d9-8e1ff5b4450f" />

Based on proximity and matching location context, the correct station was identified and tested in the required format.

## Flag

OSINT{SAINT_PHILIPPE_DU_ROULE}

## Comment

Straightforward OSINT geolocation challenge — most of the difficulty was just correctly interpreting the format and confirming the station from nearby landmarks.
