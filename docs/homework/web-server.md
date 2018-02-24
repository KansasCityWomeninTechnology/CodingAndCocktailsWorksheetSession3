# Bonus - Running a server
We can serve up web content on our own machine, but sometimes we want to make the content available publicly. In this bonus assignment we'll use a Chrome extension to act as a web server and use [ngrok](https://ngrok.com/), a command line service to expose your web server to the public securely using a HTTP tunnel.

## Prerequisites
For this assignment, find a Slack buddy so you can share content to each other!

You should also have something to share. You can share your work from the first or second session. If you don't have something to share, create a "CSS" directory in your `~/CodingAndCocktails` directory, and save the contents of CSS session answer key [from this zip file](https://github.com/KansasCityWomeninTechnology/CSSCompilerPractice/archive/2018-checkpoint-bonus-media-query.zip).

{% hint style='tip' %}
##### Hey Slacker!

Remember, we're here to help.
Join the KCWiT #codingandcocktails Slack Channel: [kcwit.slack.com](http://kcwit.slack.com)
{% endhint %}

## Install and set up a web server

1. Using Chrome, install the Chrome Web Extension [Web Server for Chrome](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb) by clicking on the link and clicking the **ADD TO CHROME** button and clicking **Add app** on the dialog that opens. It installs as a desktop application so you can run it the same way you run any of your applications or from Chrome itself.
  
   ![](images/chrome-web-server.png)

1. Launch "Web Server for Chrome" application. 

1. Click **CHOOSE FOLDER** and navigate your `~/CodingAndCocktails/CSS` or to a directory of your choosing with web content to share.
   
   ![](images/chrome-web-server-choose-folder.png)

1. Notice the **Web Server URL(s)** has a link that looks something like `http://127.0.0.1:8887`. We are serving content to our local machine using port 8887. The network address `127.0.0.1` means home and is also referred as `localhost`. You can change the port if you want to. 
   
   ![](images/chrome-web-server-port.png)

1. Click on the URL link or type in the URL manually in Chrome. You should see your content.
  
   ![](images/web-server-content.png)

You're running a local web server! Now we want to use our command line skills and make our content available using [ngrok](https://ngrok.com/).

## Create a public tunnel

1. Create an account on [ngrok](https://ngrok.com/) and follow the installation steps. Remember when you installed ngrok.

1. Open a terminal and navigate to the directory where you installed ngrok.
   {% hint style='tip' %}
Windows users - open the standard cmd shell in Cmder.
{% endhint %}


1. Run ngrok using the command for your OS. You will need to use the port you used when serving content. `./ngrok http 8887`.
  
   {% codetabs name="Mac", type="bash" -%} 
   ./ngrok http 8887
   {%- language name="Windows", type="bash" -%} 
   ngrok http 8887
   {%- endcodetabs %}

   Your command line will display the public URL of your content.
  
   ![](images/ngrok.png)

1. Navigate to either Forwarding URL in your phone. You can see your content! Share your URL with your Slack buddy or on the #codingandcocktails Slack channel. 
   {% hint style='info' %}
   You created a HTTP tunnel! A tunnel is a network link. In our case we created a tunnel from your computer to the public using the HTTP protocol. HTTP stands for **H**yper**t**ext **T**ransfer **P**rotocol and is what the internet is based on. You will learn more about protocols and the different types of protocols in the homework.
{% endhint %}

1. To exit out of ngrok, hit `CTRL+C`. When you exit out of ngrok, your public content will no longer be available.