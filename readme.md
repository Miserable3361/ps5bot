# PS5Bot

## TLDR: This code can be used by people who are not programmers. It will be easier if you know how to code, but you can do without it.

## Project Overview
This program is a modification of https://github.com/VVNoodle/PS5bot this guy's code. He made a wonderful project which taught me a lot about typescript and node.js and things I didn't even understand until I began this project. I even copied parts of his readme.md file, so don't give all the credit to me for this project. All respect and most credit to this person who archived the project now, sadly. That being said I did spend hours working on it, and I hope you make good use of it.

For right now the purpose of this bot is to help my friend buy a PS5. I am not a scammer or scalper. I am trying to help my friend who is having trouble buying a PS5 becuase of all the scammers and scalpers ruining the release of the PS5.

Keep in mind the MIT License I added, if something goes wrong and you accidentally order 10,000 PS5s, not my problem. However, I did work extra to create a good user product, and I sincerely hope it benefits you. Also, I used this code on my own credit card and I trust it to do what I said it would do. I just put the liscense to get rid of any liabilities. 

## Installation overview
I did all this on macos, linux should be no problem also. For Windows, if you're a programmer you will probably be able to manage it but I'm not going to explain how to do it for those of you who arn't programmers because I don't have a Windows machine.

The PS5Bot is not a high tech hacking bot, it is very simple. It is basically a "refresh" bot. When you turn it on, it will keep refreshing every 10 seconds until it sees the PS5 is back in stock. FOR THIS REASON, it will work better on websites that don't tell you when they will restock.

For example, on the morning of Sunday November 22nd, Best Buy dropped PS5 stock at 5 am. No one knew they were going to do it at 5 am, so this bot might have caught it.

I have been running this bot on Best Buy and Target, and have yet to actually buy a PS5 with it. However, I got it to buy paper for me from both Best Buy and Target, so we know it works.

### Installation
(Again, credit to the originator of this project, he wrote much of this part and many others.)

 1. [Install Node.js](https://nodejs.org/en/)
    1. version should be >12.9
    2. Follow the install process
 2. [Install git](https://git-scm.com/)
 3. download this project
    1. `git clone https://github.com/mmsoby/ps5bot`
 4. Open the terminal app on macos
 5. Go to project directory `cd /the/project/directory`
    1. For this don't actually type `cd /the/project/directory`
    2. Open up finder
    3. Go to the PS5Bot folder (Don't go inside it)
    4. Right click on it
    5. Hold down the option key
    6. Select `Copy "PS5Bot" as pathname`
    7. Go back to the terminal
    8. Type cd, and put one space, then paste the pathname
    9. Hit enter, nothing should happen
 6. Install `yarn` by running `npm i -g yarn`
 7. Install dependencies by running `yarn`
 8. Make CLI callable  
    `yarn link`  

## Setup

 1. Run ps5bot.
    1. Repeat step 5 of the installation process (which will bring you back into the correct folder), then type `cd bin` (hit enter)
    2. Type `./ps5bot` (hit enter)
    3. Follow the prompts, close the window when youre done
 2. Run scrape
   1. Repeat part 1 of step 1 of setup(just above).
   2. Type `./ps5bot scrape`
   3. Select the wesbites you want to scrape using the spacebar
   4. Hit enter
   5. Let it do it's thing
 

## Bot Configs

Don't worry about this part if you successfully completed setup. Just double check everything went smoothly by finding the `config.json` file and making sure your data looks correct.

Otherwise, use these instructions:

Configs are read in `config.json` file. You can either run `ps5bot` to generate a config file, or duplicate `configTemplate.json`, rename to `config.json`, and fill out the fields.

```js
{
  "cvv": "000",
  "targetEmail": "myemail@yahoo.com",
  "targetPassword": "password",
  "bestBuyEmail": "myemail@yahoo.com",
  "bestBuyPassword": "password"
}
```

- Double quotes on text is required
- Anything after the `//` are comments for clarification. Remove them if you try to copy paste this example (including the `//`).
- for Target, make sure you have no carts in your account already


Make sure to run this script and keep the terminal open if you want it to keep refreshing the page. (Basically just follow the setup steps, and don;t close any windows.

## Notes

- Make sure not to use a VPN since it will possibly trigger captcha verification.
- Make sure nothing else exists in your carts, otherwise this code will order those too!
- I recommend getting a fan and pointing it directly at your laptop to keep it cool. All this work for 7 straight days is exaughsting on a computer.
- Restart your computer to give it a break every day, then turn the code back on.

