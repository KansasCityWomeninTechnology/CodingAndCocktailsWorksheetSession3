# Homework
The more you practice, the more comfortable you’ll feel!

1. Create persistent variables and aliases (JAD TODO determine)
1. Ever wondered what _Star Wars: Episode IV_ would look like in all text? Of course you have!
   {% tabs first="Macs", second="Windows" %}

    {% content "first" %}
Type `telnet towel.blinkenlights.nl` <i class="fa fa-share fa-rotate-180"></i>.

    {% content "second" %}
Enable telnet by following the video below, then type `winpty telnet towel.blinkenlights.nl` <i class="fa fa-share fa-rotate-180"></i>.
{% raw %}
  <video id="enable-telnet" class="video-js" controls preload="auto" width="900" height="600"
  poster="enable-telnet.jpg" data-setup="{}">
  <source src="videos/enable-telnet.mp4" type='video/mp4'>
  <p class="vjs-no-js">
    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
  </video>
{% endraw %}

    {% endtabs %}

    {% hint style='info' %}
The `telnet` command uses a **protocol** that allows you to log in to another remote machine, located in this case at towel.blinkenlights.nl. A protocol is a set of procedures and rules for data transmission.

The `winpty` command allows Cmder to properly use the `telnet` command in Windows. You could also run `telnet towel.blinkenlights.nl` in the built-in Windows command prompt to get the same results.
    {% endhint %}

1. Serve content from your computer using a secure tunnel
JAD TODO - Install web server and [ngrok](). [Create an account](https://dashboard.ngrok.com/user/signup) on ngrok. Download and follow installation instructions for your OS. Use CSS code if they don't have one and serve using [instructions](https://dashboard.ngrok.com/get-started).

#### Windows users
1. JAD TODO - Rework through worksheet using Cmder's bash shell.



### More Practice

1. Work through the Command Line course on Codecademy at [https://www.codecademy.com/learn/learn-the-command-line](https://www.codecademy.com/learn/learn-the-command-line).

1. Beat the game at [http://overthewire.org/wargames/bandit/](http://overthewire.org/wargames/bandit/). You'll start by entering in the command `ssh bandit0@bandit.labs.overthewire.org` <i class="fa fa-share fa-rotate-180"></i> and typing `bandit0` as the password when prompted.
    {% hint style='info' %}
The `ssh` command stands for **s**ecure **sh**ell and is a network protocol, much like `telnet`.
    {% endhint %}
    {% hint style='tip' %}
The higher levels of this game can get decently advanced but take it step by step. You can follow the walkthrough at [https://www.yalpski.net/bandit-wargame](https://www.yalpski.net/bandit-wargame) for levels 0-17 if you need further help. Always seach the internet for anything you don't understand or need further information on!
    {% endhint %}

1. Play a fun game to sharpen your vim skills. Visit https://vim-adventures.com/.

{% hint style='tip' %}
##### Hey Slacker!

Remember, we're here to help.
Join the KCWiT #codingandcocktails Slack Channel: [kcwit.slack.com](http://kcwit.slack.com)
{% endhint %}
