# CryptoNFT
This application is a Non-commercial application. This is generated for people interested in the Motoko language, for playing around with it. The code might not be perfect.

This NFT application connects with the RC-Token, the user is able to CREATE, BUY, SELL, and MINT the NFTs.
## Technologies Used

* [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [ReactJS](https://reactjs.org/)
* [Ubuntu](https://ubuntu.com/)
* [DFX](https://smartcontracts.org/docs/current/developer-docs/quickstart/hello10mins)
* [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [Node.js](https://nodejs.org/en/)
* [Motoko](https://smartcontracts.org/docs/current/developer-docs/build/languages/motoko/)


## Getting Started
- Make sure you had the dfx installed on the computer, and also the ubuntu version of VS code is avaliable. Here is the tutorial for [Window](https://docs.google.com/document/d/e/2PACX-1vTNicu-xuf4EiLAehHIqgfpjAnPjzqMGT-xpZVvYaAWNyvzYK_Ceve_me4PVRIxpzH7ea5PAX9NxGwY/pub) and [Mac](https://docs.google.com/document/d/e/2PACX-1vTSgoWcVvuMW4Aa78MyqeK0_ZRl_MaV7rS-tdhya3jlPbSSbxczQFCohrGf87T4F7tJKXwTjT2z_QSq/pub) Credit to Dr.Angela Yu from Udemy
- To Install and Run the Project

1. start local dfx

```
dfx start --clean
```
2. Run Npm install

```
npm install
```

3. Run NPM server

```
npm start
```

4. Deploy canisters

```
dfx deploy --argument='("CryptoDunks #123", principal "trt5l-f3h3n-z6ouo-at4z7-akjoe-3tfha-zjljz-4woeh-e5i7m-jzf3j-fqe", (vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}))'
```

5. Head to localhost

http://localhost:8080/

# Creating NFT for Testing

1. Mint an NFT on the command line to get NFT into mapOfNFTs:

```
dfx canister call opend mint '(vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}, "CryptoCat #123")'
```

2. List the item into mapOfListings:

```
dfx canister call opend listItem '(principal "<REPLACE WITH NFT CANISTER ID>", 2)'
```

3. Get OpenD canister ID:
 
```
dfx canister id opend
```

4. Transfer NFT to OpenD:

```
dfx canister call <REPLACE WITH NFT CANISTER ID> transferOwnership '(principal "<REPLACE WITH THE ID FROM STEP 3>", true)'
```

# Connecting to the Token Canister


1. Copy over the token declarations folder

2. Set the token canister id into the <REPLACE WITH TOKEN CANISTER ID>

```
const dangPrincipal = Principal.fromText("<REPLACE WITH TOKEN CANISTER ID>");
```

## User Stories

As a user, I want to be able to create an NFT for se

As a user, I want to be able to buy the NFT

As a user, I want to be able to sell the NFT

As a user, I want to be able to see the NFTs I had


## Design Layout
  
![image](https://user-images.githubusercontent.com/87446864/168520087-ffeff3e1-190c-4a0d-9aae-6e2c0cf471d7.png)
  ![image](https://user-images.githubusercontent.com/87446864/168520223-e7f980e7-1651-4988-af4a-8dd66c31171f.png)




## Authors

* **Panta Huang** 
- [Github](https://github.com/willyhuang18)
- [LinkedIn](https://www.linkedin.com/feed/)

- Credit to Dr.Angela Yu from Udemy


## License

This project is licensed under the MIT License 
