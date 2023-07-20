Hi @matavatar , i've gone through the Todo on GH and would like to ask a few things

- **Dashboard**
  - Global features
      - Enable/Disable each "Command" 
      - Control all comads
      - **QUESTION**
          - the dashboard should be in website admin or a separate website
              - separate is easier to maintain
  - **Steam Keys manager** ( pls tell / add / remove features you need)
      -  **QUESTIONS**
          - Being able to put a set amount of steam key (from text file or xls).
              - What if the amount of people that sign up is more than available keys ?
  - **Playtest creator**
      - Info
          - Show amount of people that registered
          - allow to remove or add people manually
          - add priority to user
          - ban person from registering
          - show how many times a person has signed up
          - preform batch operations 
              -  example remove a bunch of users at once, (select all )
          - Track if the person actually used the key ?
      - Each playtest will be a "Session" and all will be shown separately
      - Create a playtest (set date / number of player / playtest password / connect a form to a playtest)
      - add a name to the session ( so that later a channel with same name can be created ? )
      - Upload Playtest PDF presentation.
      - Button to start sending invitations to selected from a form
          - this will send a DM ?
          - what if the user has disabled DM ?
      - Confirmation button : “Please confirm your participation to the playtest -at the specific date-”
          - If the user says no, remove them from this session and give key to someone else ?
      - 5 minutes prior to the playtest give playtest password + link to a specific discord voice channel to join
          - Playtest Password ?
          - Channel is created by the bot or admin ?
  - **Forms creator**
      - the examples in the github are not opening pls update 
	      - <https://github.com/DeepWorlds/BL_Discord_Bot/issues/3>
      - track all forms created by bot ?
      - add ability to remove a form ?
      - Add ability to find STEAM ID from url basically ( [https://steamid.pro/](https://steamid.pro/ "https://steamid.pro/") ) ?
  -  **Influencer FINDER**
          -  Can set what plateforms are being looked at by the bot (check box so can be multiple at a time) Twitter / Youtube / Twitch / Kick / Instagram
              - will need a list of all platforms you want to get info for

# Timeline
- Till when you want these features be done ?

This is the first round of questions this will give me a general understanding of the scale of things required to do


# Price distribution
- Dashboard (1.5 + 2k + 1.8k + 500 = 6k)
	- Base 1.7k ( login, enable/disable command, website, non-responsive)
		- this is one time
	- Playtest (  2k ) ( includes bot and admin panel)
		- Steam keys importer ( 200 )
		- manager ( 1.8k )
	- Form Creator ( 1.8k )
		- Base  ( 1k ) 
			- Form Creation
			- Form control
			- Edit and add new field
			- View entries for each form
			- Which channel to send the form to
			- Watch the message
		- Ability to edit and add inputs on fly (500)
			- only text and number inputs
				- ( 100  extra ) for drop-down input
			- Adding this allows you to create any amount of forms 
		-  Apply form (150)
		- feedback form (150)
		- Form entries
	- Form and Playtest data saving and export (500)
	
- These will be available for all these and next commands, for free
	- Hosting setup and config
	- 10 free small revisions ( typo, text change )
	- 2 free major revisions ( change how a command works )
	- Regular maintenance