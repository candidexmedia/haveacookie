<h1 align="center" style="border-bottom: none">
    <b><a href="#">Have a Cookie!</a> 🍪 (or any emoji)</b><br>
  
 <br>
</h1>

<p align="center">
The Open Source HeyTaco! alternative for Discord that fosters better communities through rewards and recognition. 
</p>

<p align="center">
    <a href="#"><b>Website</b></a> •
    <a href="#"><b>Twitter</b></a> •
    <a href="#"><b>Documentation</b></a>
</p>  

# (PROMO VIDEO)

# Features
### Give kudos to your community-members
- ⚡ ...
- ⚡ ...

### Redeem points for prizes
- ⚡ ...
- ⚡ ...

### Customize everything!
- ⚡ Don't like the "cookie" 🍪 points? Give your team a 🥭, 🥝, 👍, 🍔, 🙌, etc. instead! The choice of emoji is yours.
- ⚡ Create your own rewards: give it a name, set the "price", provide instructions, and more
- ⚡ Set your own limit for the amount of tacos your server members can give per day.
- ⚡ Choose your prefix

### In public or in private: you choose!
- ⚡ ...
- ⚡ ...

# Screenshots

# Getting Started ([Railway.app](https://railway.app?referralCode=7ENqQl))
## Video Tutorial

## Written Instructions ([Railway.app](https://railway.app?referralCode=7ENqQl))
### Creating your Discord Bot ([based on discordpy docs](https://discordpy.readthedocs.io/en/latest/discord.html))
- Make sure you’re logged on to the [Discord website](https://discord.com/).
- Navigate to the [application page](https://discord.com/developers/applications).
- Click on the blue "New application" button at the top-right.
- Give the application a name and click “Create”.
- In the left sidebar, click on the "Bot" tab and select "Add bot"
- Give your bot a cool username and icon. This is what how it'll appear in the server.
- Take note of the bot token, as you will need to add it to your code in the next section.
- You can leave the remaining "Authorization Flow" and "Privileged Gateway Intents" options unchecked, unless you believe they apply to your project.
- It's now time to invite your bot to your server. Head to the left sidebar and click on OAuth2 > URL Generator.
- In "Scopes", check the "bot" option
- Under "Bot Permissions", select "Administrator". I have not tested other permissions, but feel free to select other ones if you wish.
- Copy the Generated URL, and open the link.
- Add the bot to the respective server.

### Creating your Code Repository
1. Create a private clone of [this repository](https://github.com/havecookie/haveacookie) on GitHub. Make sure this repo is set to private, as you will be adding senditive information in the later steps.
2. In your repo, select the `data` folder, and click on [`config.json`](https://github.com/havecookie/haveacookie/blob/main/data/config.json)
3. Edit the variables for your custom bot. You can customize the emoji, prefix, max per day, prizes, and prize channel.
4. IMPORTANT: Make sure to add the bot token (from the previous section), and database URL (next section)

### Hosting your bot
1. If you don't have one already, [create a Railway.app account](https://railway.app?referralCode=7ENqQl)
2. Create a new Project, and select "Deploy from GitHub repo".
3. In the same "New Project" window, also select "Provision PostgreSQL".
4. Once everything is deployed in Railway, select the project and click on the rectangle with the GitHub repo's name.
5. On the right window, click on the "Settings" tab, and in the "Environment" section, make sure the automatic deployment trigger is enabled.
6. Afterwards, click on the PostgreSQL rectangle.
7. On the right window, click on the "Connect" tab, and copy the "Postgres Connection URL".

### Updating code with Database URL
1. In your GitHub repository, return to [`config.json`](https://github.com/havecookie/haveacookie/blob/main/data/config.json) and paste the Postgres Connection URL as the value for `"databaseUrl" :`. For example: 
2. Saving these changes will trigger the deployment of an updated Railway project.
3. Your bot should now be live and working.

### Testing the Bot
1. Give a reward: In any channel where the bot is present, `@` mention a fellow user followed by the emoji. For example, `"thanks for the help @candidexmedia :cookie:"`
2. List of Prizes: Direct message the bot using your prefix set in [`config.json`](https://github.com/havecookie/haveacookie/blob/main/data/config.json) followed by `prizes` (no space) (ie: "`!prizes`").
2. Purchase a Prize: Direct message the bot using your prefix set in [`config.json`](https://github.com/havecookie/haveacookie/blob/main/data/config.json) followed by `prizes` and the prize number (ie: "`!prizes 1`" for the first prize listed in the prize list).
3. Leaderboard + Check Balance: `@` mention the bot in any channel where it's present.

# About the project
I commissioned this bot from a freelancer on Fiverr named [mdaniels6758](www.fiverr.com/mdaniels6758). I made some modifications and decided to open source the project in the hopes that it will benefit other Discord users, and that improvements can be brought to the project collectively.

# Wishlist / Bugs to Fix
Help, Suggestions, and Pull Requests are much appreciated!
Consult the list of bugs and feature requests here: https://github.com/havecookie/haveacookie/issues

# Support
Do you enjoy this software? If so, consider supporting me so that I can bring more open source ideas and tutorials to life! <br><br>
https://ko-fi.com/candidexmedia <br><br>
<a href='https://ko-fi.com/O4O61QG9T' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://cdn.ko-fi.com/cdn/kofi5.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
<img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg">
