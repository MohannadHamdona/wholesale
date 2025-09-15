# WIT Conversation Platform

##Web Channel configuration
WIT Conversation Platform Web Channel allows to run bots in any authorized web page.

##Prerequisites
Before starting the web channel configuration please ensure that you have your domain in the allowed domains list (in the web channel configuration page on your bot control panel).
Also ensure that you have the following files (under the code folder):

- chat.css - css required to style the chat window and messages
- lightbox.css - css required to style the lightbox to display received images in a bigger window
- toggle.css - css required to style the toggle button
- wbe-iframes.css - css to style the iframes
- toggle.html - the page loaded by one of our iframes
- sdw-properties.json - configuration file for the web channel
- main.[hash].js - logical assets of the web channel

###Configuration
To configure your bot please go to the sdw-properties.json file and update the following variables with your bot configuration (obtained in the WIT Conversation Platform web channel configuration page):

- serverUrl - the WIT Conversation Platform gateway versioned url
- botToken - the bot's access token
- botName - the bot's id (obtained in the Control Panel page)

###Installing
To integrate the web channel in your web page please:

- Link the web channel assets and configuration file
- Copy and past the following HTML on the page, before body HTML tag ending:
- Edit the css path and the page path to the `wbe-iframes.css` path and the `toggle.html` path

```
<link rel="stylesheet" type="text/css" href="[CSS-PATH]">
  <iframe id="wbe-sdw-bot" src="[PAGE-PATH]"></iframe>
```

###Running
To see the bot in action please clean your web page cache and refresh the page.
Before start testing the bot please go to the the WIT Conversation Platform and make sure that your bot is running and the page's domain is already defined in the bot channel configuration.

###Assistance
If you need some help, we are here to help: botengine.support@wit-software.com
