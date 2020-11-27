#PS5Bot

##TLDR: This code can be used by people who are not programmers. It will be easier if you know how to code, but you can do without it.

##Project Overview
This program is a modification of https://github.com/VVNoodle/PS5bot this guy's code. He made a wonderful project which taught me a lot about typescript and node.js and things I didn't even understand until I began this project. I even copied parts of his readme.md file, so don't give all the credit to me for this project. All respect and most credit to this person who archived the project now, sadly. That being said I did spend hours working on it, and I hope you make good use of it.

For right now the purpose of this bot is to help my friend buy a PS5. I am not a scammer or scalper. I am trying to help my friend who is having trouble buying a PS5 becuase of all the scammers and scalpers ruining the release of the PS5.

## Installation overview
I did all this on macos, linux should be no problem also. For Windows, if you're a programmer you will probably be able to manage it but I'm not going to explain how to do it for those of you who arn't programmers because I don't have a Windows machine.

The PS5Bot is not a high tech hacking bot, it is very simple. It is basically a "refresh" bot. When you turn it on, it will keep refreshing every 10 seconds until it sees the PS5 is back in stock. FOR THIS REASON, it will work better on websites that don't tell you when they will restock.

For example, on the morning of Sunday November 22nd, Best Buy dropped PS5 stock at 5 am. No one knew they were going to do it at 5 am, so this bot might have caught it.

I have been running this bot on Best Buy and Target, and have yet to actually buy a PS5 with it. However, I got it to buy paper for me from both Best Buy and Target, so we know it works.

### Installation

 1. [Install Node.js](https://nodejs.org/en/)
    1. version should be >12.9
 2. [Install git](https://git-scm.com/)
 3. download this project
    1. `git clone https://github.com/VVNoodle/PS5bot`
 4. Open up a terminal
 5. go to project directory `cd /the/project/directory`
 6. Install `yarn` by running `npm i -g yarn`
 7. Install dependencies by running `yarn`
 8. Make CLI callable  
    `yarn link`  

## Setup

 1. Run ps5bot. You'll be prompted to fill in required checkout info  
    `ps5bot`  
    **Note: Below steps are still TODO**  
 2. Run scraper
    `ps5bot scrape`
    - you will be asked to select the sites to run the bot. If you don't select anything, it will try to run on all websites.

## Bot Configs

Configs are read in `config.json` file. You can either run `ps5bot` to generate a config file, or duplicate `configTemplate.json`, rename to `config.json`, and fill out the fields.

```js
{
  "firstName": "Qwer",
  "lastName": "Ty",
  "phoneNumber": "8011111111",
  "email": "email@example.com",
  "state": "State",
  "city": "Random City",
  "address": "2353 Running Water Ct.",
  "zipCode": "95054",
  "creditCardNumber": "0101101010101",
  "expirationMonth": "10",
  "expirationYear": "2022",
  "cvv": "000",
  "targetEmail": "email2@example.com",
  "targetPassword": "1312321"
}
```

- Double quotes on text is required
- Anything after the `//` are comments for clarification. Remove them if you try to copy paste this example (including the `//`).
- for Target, make sure you have no carts in your account already

### Credit Cards supported

| Site               | Cards                                        |
|--------------------|----------------------------------------------|
| PlayStation Direct | MasterCard, Visa, Discover                   |
| Walmart            | MasterCard, Visa, Discover, American Express |
| Target             | MasterCard, Visa, Discover, American Express |

Make sure to run this script and keep the terminal open around the time of the schedule

## Notes

- Make sure not to use a VPN since it will possibly trigger captcha verification.
- There's a chance WalMart checkout ask for captcha after entering address. If this is the case, bot will pause. As soon as you complete them, bot will resume.
- You need a login for Target. And make sure no existing carts.

PS5bot exists to:

- practice web scraping and to
- buy a **single** PS5 for myself  
The second point is fair imo since it's pretty much an automated version of constantly clicking refresh to buy stuff.  
Also: This is not intended to scalp massive quantities of PS5s. That shit aint cool.
