1. Open iTerm2 on a Mac or Cmder in Windows.
1. Type `pwd` <i class="fa fa-share fa-rotate-180"></i> in your CLI to see your current user's home directory. `pwd` stands for **p**rint **w**orking **d**irectory.
   {% hint style='info' %}
The <i class="fa fa-share fa-rotate-180"></i> icon tells you when to press `Enter`.
    {% endhint %}
1. Type `ls` <i class="fa fa-share fa-rotate-180"></i> to see the contents of your current directory.
1. Type `ls -al` <i class="fa fa-share fa-rotate-180"></i> and compare it to your previous output.  You should see more information and all files, including hidden files.
1. Next, enter in `cd CodingAndCocktails` <i class="fa fa-share fa-rotate-180"></i> to **c**hange **d**irectory into the "CodingAndCocktails" directory listed in the output of `ls`.
   {% codetabs name="Mac", type="bash" -%}
cd ~
{%- language name="Windows", type="bash" -%}
cd %USERPROFILE%
{%- language name="Chromebooks", type="bash" -%}
cd ~
{%- endcodetabs %}
    {% hint style='info' %}
If the CodingAndCocktails folder doesn't exist, create it using `mkdir CodingAndCocktails`. Make sure you switch into your home folder by typing `cd ~` first. You should have done this when following [**The Tools**](http://bit.ly/CnCTheTools) worksheet.
    {% endhint %}
    {% hint style='tip' %}
Both Cmder and oh-my-zsh use formatting to distinguish between what's a directory and what's a file. You won't be able to `cd` into a file.
    {% endhint %}
1. Once you've moved into a new directory, type `ls -al` <i class="fa fa-share fa-rotate-180"></i> again to see what's listed there.
7. Let's move back up one directory. To do this, type `cd ..` <i class="fa fa-share fa-rotate-180"></i>.
    {% hint style='info' %}
The **..** is a shortcut for the parent directory  much like the **~** is a shortcut for your home directory. A parent directory would be the directory that contains your current directory. No matter where you are, `cd ..` or `cd ~` are always valid commands.
    {% endhint %}

#### Tab Completion

You'll also want to utilize **tab completion** with your **tab** key and your **up/down** arrow keys. Tab completion will allow you to enter in part of a filename or directory name and then it'll be completed for you. Your up/down arrow keys will allow you to scroll through previous commands.

1. Let's switch back to the home directory by typing `cd ~` ![](images/enter.png).
2. Enter in `cd Cod` then stop and hit your `tab` key. Tab completion will find your CodingAndCocktails folder and enter the rest in for you!

Now try navigating around on your own! See the video below for some help. You can watch it in fullscreen as well. To download the video, right-click and click "Save video as...".

{% raw %}
  <video id="CLI_Part1" class="video-js" controls preload="auto" width="900" height="600"
  poster="CLI_Part1.jpg" data-setup="{}">
  <source src="videos/CLI_Part1.mp4" type='video/mp4'>
  <p class="vjs-no-js">
    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
  </video>
{% endraw %}