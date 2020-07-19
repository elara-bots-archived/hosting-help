# Hosting Help

This is a work in progress hosting help list. I'll add onto it whenever I have the time.






# Heroku

### Notes
1) These steps might change in the future.

2) This will go over how to setup just about everything.

3) Unless you add a credit card to your account you'll only have 550 Dyno hours for the bot/project to run. You'd have to create another account to run the bot/project for the whole month.

4) The more apps you put on one account the more your Dyno hours will go down.

Step 1: Go to your project and add `Procfile` with the contents of 
```bash
worker: node index.js
```
(yes this will work with any coding language that Heroku supports, just replace node/js with your coding language startup stuff, if your main file isn't `index.js` just change index.js to whatever you called your main file)

Step 2: Go to https://heroku.com and setup an account.

Step 3: Once you create an account, click on `New` then `Create new app` then put in the name you want to set for the app

Step 4: Once you created the app, go to GitHub or if you're willing to do Heroku CLI then do that. But we'll be covering only GitHub for the moment. Click on the `GitHub` tab in `Deploy` you'll need to connect your Heroku account to your GitHub account to do this. But once you've authorized it.. you should be able to search for your project name. 
Once you connect that project to Heroku press the branch you want to use then press **Deploy Branch** and wait until that is finished.

Step 5: Go the **Resources** tab and switch OFF the web worker and switch on your other worker. 

Step 6: To setup all of the `.env` stuff on Heroku you have to go to the `Settings` tab then scroll down until you see **Reveal Config Vars** then put all of your .env fields into there (see image below)

Step 7: To view the logs click **More** then **View Logs**


### Images
Config Vars: 

![config vars](https://i.imgur.com/Oo0yBju.png)


# If you have any questions or issues
Join here: https://superchiefyt.xyz/support 
