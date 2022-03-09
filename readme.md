# School Discord Bot
Good for verifying a user's email before giving access to the server, and giving roles for 7th-12th grade.
### Instructions
1. Copy the repo <br>
`git clone https://github.com/svalencia014/fcBot.git` <br>
or <br>
`gh repo clone svalencia014/schoolBot` <br>

2. Go into the directory <br>
`cd schoolBot`

3. Install packages <br>
`./setup.sh`

4. Edit the last line of bot.js with your discord token (from discord.com/developers) <br>
line 36: `client.login("Insert your token here");`

5. Sign up for a [sendGrid](https://sendgrid.com/) account and input your api token in /commands/verify.js (Found on the integration page, where you send your first email) <br>
line 3: `sgMail.setApiKey('Your api key here');`

6. Skim though verify.js and look for any "Discord name here" or "your email" and replace them accordingly. <br>
`lines 18, 27, 51, 55, 58, 116, 120`

7. Run with node <br>
`node .`