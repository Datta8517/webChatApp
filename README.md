# webChatApp

# Project is live on the given link:👇👇👇
https://eng-group-chat.netlify.app/		(Hosted on Netlify)

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
    	
    -	Invite friends Direct
    o	Select friend
    o	Click on the invite
    o	Message to the friend
    -	Group Messaging
    o	Select friend 
    o	Create a group name
    o	Save 
    o	Message in group
    
    -	Access functions like sharing documents, contacts, emojis, gifs, and tagging to the messages through ChannelInner file << components << src << client


# 3.2 RESULTS:
	Hence, we successfully developed an API that processes and serves data from the app present on different platforms. 	
![SignUpForm](https://github.com/Datta8517/webChatApp/assets/84066284/a7c7b52f-5417-4326-8032-b3a1063fdb6f)

						fig a. SignUp Page


![LoginForm](https://github.com/Datta8517/webChatApp/assets/84066284/70fcdbfb-a261-4792-8e00-0bd7bb6b2923)

						fig b. Login Page





![MessageTexting](https://github.com/Datta8517/webChatApp/assets/84066284/92cf843b-544a-4df9-986a-01504ddc8ac4)

# Message Texting: 
The user can type and send text messages to the other user instantly. This has been accomplished by socket connection. The stream-chat dependency gets the sending socket used for the connection. The text messages are sent through the socket. The key listener has been implemented on the bottom-most window where a user types the message. On the press of the Enter key, the text message is sent to the other user and displayed over the text area of both the user. The receive function on the other side text messages and sends it to the text-area of the receiving user. In this way the texting has been implemented in this application.






 
![ThreadingMessage](https://github.com/Datta8517/webChatApp/assets/84066284/3ffb4aa2-7117-4eea-a2b2-e365befc1474)			

# Threading:  
Threads preserve meaningful context and organize conversations. A thread encourages open discussion about topics without distracting others. Threads give you a way to get more clarity, without starting a new DM. Your threads make it easier to track information by looking at specific conversations. Threads keep announcement channels clear of extra clutter. Only those actively participating in a thread get notified; reducing notification overload. Threads are sticky. When you share a message, threaded replies share too. 

