# BabyOSINT
> Bored at work, so here's what my window gets to stare at all day. I wonder what is my current location's plus code. Flag format: sunctf25{123CTF}
> 

- `Challenge Type: OSINT`
- `Points: 80`
- `Flag: sunctf25{4PR9}`

# Solution

### 1. Examining the File Contents
We are provided with an image file, `photo.jpg` to be analyzed.

<img width="1440" height="762" alt="image" src="https://github.com/user-attachments/assets/d6c6c2e2-f183-4f82-ba8b-bc27a8d38062" />

### 2. Examining the Challenge's Description
Firstly, the challenge's description is analyzed to search for potential information and hints. 

According to the challenge's description, we are required to find the challenge creator's location plus code based on the photo given. We are also provided with additional information that the creator took the photo when he is bored at work, signifying that the photo is taken from his workplace.

<img width="516" height="368" alt="image" src="https://github.com/user-attachments/assets/49911fcf-3f4f-4890-8994-a76a065a8f61" />

### 3. Searching for the Location
With the required information, I started off by searching for the creator's workplace location by conducting a simple online search on the challenge creator's username, `warlocksmurf` and it returned a list of results related to CTFs. 

<img width="1931" height="932" alt="image" src="https://github.com/user-attachments/assets/6c0a1561-ef1d-4cbd-bf5e-05cdabe8c12e" />

Upon clicking in the first result, being the github profile. I have managed to collect several important information, such as the:

- `challenge's creator real name: Robbin`
- `challenge's creator profile picture: blue crab`
- `challenge's creator potential working location: Gen Digital`

<img width="1919" height="932" alt="image" src="https://github.com/user-attachments/assets/b4600b02-b320-4835-a2fa-27f2c51eecb0" />

With the newly obtained information, I conducted a simple validation test by searching for the challenge creator's linkedin profile using the name `Robbin` followed by the potential working location: `Gen Digital`. With that, I managed to find out the profile which fulfills all the information.

<img width="868" height="525" alt="image" src="https://github.com/user-attachments/assets/c41814f0-90fb-4c37-b204-45488d6b535c" />

Upon scrolling down the profile, I have obtained more information in regards to which company the creator is working at. In this case, the challenge creator is working in Gen Digital, and an additional information is also provided which states that MoneyLion is now under Gen Digital, signifying his previous working company is MoneyLion.

<img width="851" height="675" alt="Screen Shot 09-01-25 at 06 47 PM" src="https://github.com/user-attachments/assets/b1c79dc2-3f7d-47e9-8beb-91ba0182dce3" />

I then proceeded to search for the company's location address through a simple google search. The first search of `Gen Digital Malaysia` did not return any address.

<img width="1929" height="933" alt="image" src="https://github.com/user-attachments/assets/d3e5d4f9-344c-47fa-8336-b23ef2bf9469" />

I then searched for MoneyLion Malaysia as MoneyLion is now under Gen Digital and it returned the required location address

<img width="1929" height="933" alt="image" src="https://github.com/user-attachments/assets/38ef2c13-8d4d-4ba2-a58c-226041ad1c05" />

### 4. Identifying the location's plus code
Once the location address is obtained, I then inserted the location address into Google Plus Code Website, which returned the plus code of `4PR9`. Thus, the obtained flag will be `sunctf{4PR9}`

<img width="1929" height="933" alt="image" src="https://github.com/user-attachments/assets/1d0e93cd-4a28-4764-b088-62ab382207df" />

