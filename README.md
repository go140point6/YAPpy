# Yet Another Price Bot (YAPpy) 
Simple XRPL Dex price bot for discord

To Run Script:

1. Install Node JS and NPM (minimum version 16.x):

        (https://nodejs.org/en/download/)
        
2. Clone the repository

        git clone https://github.com/go140point6/YAPpy.git
        
3. Open a command prompt, powershell or terminal window. Navigate to the script folder and issue the npm install command:

        npm install
        
4. Create a new application and bot on discord. Make note of the bot token and client ID.

5. Open constants.js in VS Code or Notepad (or be cool like me and use Vim) and replace your variables as needed.  The ./tokens folder as a growing list of tokens I like already filled out. 

	//******************* REPLACE THESE VARIABLES *********************/
	const TOKEN_CURRENCY_NAME = 'xKangaMK1'; //Name of currency
	const TOKEN_CURRENCY = '784B616E67614D4B310000000000000000000000'; //40 character 160 bit hex currency code
	const TOKEN_ISSUER = 'rPwdrA6YFGR6k5rPyT6QPx7MrQAavUtyz5'; //Token Issuer
	const AVATAR_URL = 'https://secure.gravatar.com/avatar/C270F8CB93F1E0D895AB0DD40AE50F1F?d=mm&s=173'; //Avatar URL
	const UPDATE_FREQUENCY = 240; //Update Frequency in seconds
	//*************************************************************** */

6. Create a new file in the YAPpy directory called ".env" and add the following contents, replacing the 2 variables with your bot token and server ID

        DISCORD_BOT_TOKEN=*****YOUR BOT TOKEN HERE******
        DISCORD_SERVER_ID=*****DISCORD SERVER ID HERE*****
        
7. Invite your bot to the server of your choice with an authorize link below. Replace [***ClientID***] with your application Client ID you generated in discord

        https://discord.com/api/oauth2/authorize?client_id=[***ClientID HERE***]&permissions=0&scope=bot%20applications.commands
        

8. Start the script:

        node index.js
