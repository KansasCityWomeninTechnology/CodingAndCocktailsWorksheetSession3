# Part 1: Navigating & Basics

---

#### Where am I?!?

The command line is just another way to navigate your computer's directory structure and issue commands. Typically, you have a **GUI**, or **G**raphical **U**ser **I**nterface, available to you. So why use a **CLI **\(**C**ommand **L**ine **I**nterface\)? Well, believe it or not, it's faster, uses fewer resources, and is much more powerful than a GUI! Let's take a look at how to orient yourself at the command line.

When you first open iTerm2 in a Mac or Git Bash in Windows, you'll likely be in your home directory at what's called a **prompt** in a **shell**. A shell is the program that provides the text-only user interface. The prompt is what's waiting on you to provide input to the shell in the form of a command. You probably will see a **~** in your CLI as well. This is a shortcut for your home directory.

Let's find out what the full path to the ~ directory looks like with the `pwd` command, which stands for **p**resent **w**orking **d**irectory. When you type `pwd` and hit enter, you should see your current user's home directory listed.

Let's try out some more commands!

1. Type `ls`** **to see the contents of your current directory. Typing `ls -al`** **will give you more information and show you **a**ll files, including hidden files.
2. Next, use `cd` to change directory into one that was listed in the output of `ls`.
   {% hint style='tip' %}
   * Both Git Bash and oh-my-zsh use formatting to distinguish between what's a directory and what's a file. You won't be able to `cd` into a file.
   {% endhint %}

3. Once you've moved into a new directory, type `ls -al`** **again to see what's listed there.
4. Let's move back up one directory. To do this, type `cd ..`.
   {% hint style='info' %}
   * The '**..**' is a shortcut for the parent directory  much like the **~** is a shortcut for your home directory. A parent directory would be the directory that contains your current directory. No matter where you are, `cd ..`** **or `cd ~` are always valid commands.
   {% endhint %}

You'll also want to utilize **tab completion** with your **tab** key and your **up/down** arrow keys. Tab completion will allow you to enter in part of a filename or directory name and then it'll be completed it for you. Your up/down arrow keys will allow you to scroll through previous commands.

Now try navigating around on your own! See the video below for some help. You can watch it in fullscreen or download it as well.

{% raw %}
  <video id="CLI01" class="video-js" controls preload="auto" width="700" height="450"
  poster="CLI01.jpg" data-setup="{}">
  <source src="videos/CLI01.webm" type='video/webm'>
  <p class="vjs-no-js">
    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
  </video>
{% endraw %}

