﻿# webChatApp


# IMPLEMENATAION:

# 1. Implementation of the getstream.io (for Authentication)
	 - API key, API secrete, API ID helps to get an authentication for website. It links database to the Sign-Up page
	- Implements dependencies like stream-chat, stream-chat-react, universal-cookie to access the Channel list, Channel Container, Channel
	- Dependency universal-cookie use to set the info in client site also to get same info in database as a data format
	- creating get and post requests for basic routes
	-  data store
 
# 2. Implementation of Twilio (for SMS, alert & notification)
	- Via code using JavaScript
	- Login in Twilio.com site to access the dashboard
	-Store the data of ACCOUNT_SID, AUTH_TOKEN, SERVICE_SID in server/.eve file
	- access the above info in <server>/<index.js> to connect Twilio to the server

# 3. Implementation of Heroku (Deployment of the Web App)
	- Run Heroku in cd . /<server>
	- Login in Heroku
	- .gitINGNORE the node_modules from the server folder
	- Add all the backend to the Heroku >> 
    <server> git .add
    <server> git commit
    <server> git push Heroku master
	- Click on Open App on the Heroku
	- Screen shows “Hello, World!”, procedure is successful
	- Copy the site link and past it in the getstream.io >> 
		Overview -> Real Time -> Webhooks -> past link in <webhook URL>
    - Paste same link as const URL = ‘link/auth’; in client /<src>/ <Components>/ <Auth.jsx> -> const handleSubmit

# 4. Implementation of netlify

    -	Deploy the frontend part by implementing netlify 
    -	Login in the netlify site 
    -	Create build folder in client folder which store the frontend details
    -	To create build folder run code: cd client >> npm run build
    -	Simply drag and drop the build folder in netlify site 
    -	Edit name of the site
    Click option >> change name >> save 
    -	Now site is live 


# Execute the site through code:
    -	Open terminal in client 
    Run >> npm start
    -	If (Sign In)? Login: Sign Up
    Fill info:
    	Get full name
    	Get Username
    	Get Phone number
    	Get Avatar URL
    	Get Password
    	Get confirm password
    	
    -	Invite friend Direct
    o	Select friend
    o	Click on invite
    o	Message to the friend
    -	Group Messaging
    o	Select friend 
    o	Create group name
    o	Save 
    o	Message in group
    
    -	Access function like sharing documents, contact, emojis, gif, tagging to the messages through ChannelInner file << components << src << client
