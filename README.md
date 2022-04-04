# PuuCraft Place Bot

The bot for PuuCraft and their allies, forked from PlaceNL! This bot connects with the [command server](https://github.com/Indicardo/Commando) and gets its orders from there. You can see the order history [here](https://placebot.oc.tc/).

## User script bot

### Installation instructions

before you start, make sure your cooldown has run out!

1. Install the [Tampermonkey](https://www.tampermonkey.net/) browser extensbion.
2. Click on this link: [https://github.com/minipasila/PlaceBot/raw/master/placebot.user.js](https://github.com/minipasila/PlaceBot/raw/master/placebot.user.js). If everything went well you'll see Tampermonkey ask you to add it. Click **Install**.
3. Reload your **r/place** tab. If everything went well, you'll see "Getting access token..." in the top right of your screen. The bot is now active, You'll be able to see what the bot is doing through these messages.

### Cons of this bot

- When the bot places a pixel, it will look as if it wasn't placed, while the bot has already done that (and thus you're in cooldown). You can see the cooldown in the topright of your screen.

## Headless bot

### How to get reddit_session cookie

**NOTE: People have reported that this is annoying to do on Chrome because texts get unselected. Therefore we recommend that you use Firefox.**

1. Go to [r/place](https://reddit.com/r/place)
2. Open dev tools and go to the network tab
3. Refresh the page
4. Click on the first request to reddit.com/r/place (See image)
   ![Screenshot_20220403_165251](https://user-images.githubusercontent.com/9784257/161433856-27ef7e7c-7f00-4b37-b274-4199ea919aa9.png)
5. Go to the tab called `Cookies`
6. Copy the value of the `reddit_session` cookie

### Installation instructions

1. Install [NodeJS](https://nodejs.org/).
2. Download the bot via [this link](https://github.com/PuuCraft/PlaceBot/archive/refs/heads/master.zip), or clone the repository.
3. Extract the bot anywhere on your desktop
4. Open a command prompt/terminal in this folder

   - **Windows**: Shift + right click on the folder -> Click on "open Powershell here"
   - **Mac**: Open the terminal, usually located in Launchpad -> Other -> Terminal
   - **Linux**: Is this necessary?

5. Install the dependencies: `npm i`
6. Execute the bot by running `node bot.js SESSION_COOKIE_HERE`. Alternatively, you can create a .env file and add a bunch of reddit accounts, following the example in `.env.example`.
7. BONUS: You can repeat these steps for any amount of accounts you'd want. Keep in mind to use different accounts.
