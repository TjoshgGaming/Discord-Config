# Creating Files
This will show you how to create a discord config file.

So first you gonna create these files to run your bot!

so create a folder on your desktop, then open command prompt and type:

Discord Bot


so after that open it and open command prompt type this:


cd C:\users\%username%\desktop\Discord Bot\

npm install discord.io

npm init





then after that let it run
once it was run you should see files in your folder.

# Coding

So you need to code?

create a bot at **Discord developer portal (https://discord.com/developers/applications)

Then we will get a token at the bot menu.

create a file called "bot.js"
make sure it is not a text file like "bot.js.txt"
in that, open it with notepad.

put this in:



var Discord = require('discord.io');

var bot = new Discord.Client({
    token: "",
    autorun: true
});

bot.on('ready', function() {
    console.log('Logged in as %s - %s\n', bot.username, bot.id);
});

bot.on('message', function(user, userID, channelID, message, event) {
    if (message === "ping") {
        bot.sendMessage({
            to: channelID,
            message: "pong"
        });
    }
});



put your token in "token: "YOUR_TOKEN"

then run it with node.js


if you do not have node.js

install it from **node.js.org(node.js.org)

