# Part 1: Navigating & Basics

---

#### Where am I?!?

The command line is just another way to navigate your computer's directory structure and issue commands. Typically, you have a **GUI**, or **G**raphical **U**ser **I**nterface, available to you. So why use a **CLI **\(**C**ommand **L**ine **I**nterface\)? Well, believe it or not, it's faster, uses less resources, and is much more powerful than a GUI! Let's take a look at how to orient yourself at the command line.

When you first open iTerm2 in a Mac or Git Bash in Windows, you'll likely be in your home directory at what's called a **prompt**. The prompt is what's waiting on you to provide input in the form of a command. You probably will see a **~** in your CLI as well, which is a shortcut for your home directory. Let's find out what the full path to the ~ directory looks like with the `pwd` command, which stands for **p**resent **w**orking **d**irectory. When you type `pwd` and hit enter, you should see your current user's home directory listed.

Let's try out some more commands!

1. Type `ls`** **to see the contents of your current directory. Typing `ls -al`** **will give you more information and show you hidden files.
2. Next, use `cd` to change directory into one that was listed with `ls`.
   * Both Git Bash and oh-my-zsh use formatting to distinguish between what's a directory and what's a file. You won't be able to `cd` into a file.
3. Once you've moved into a new directory, type `ls -al`** **again to see what's listed there.
4. Let's move back up one directory. To do this, type `cd ..`. 
   * The '**..**' is a shortcut for the parent directory, much like the **~** is a shortcut for your home directory. No matter where you are, `cd ..`** **or `cd ~` are always valid commands.

You'll also want to utilize **tab completion** with your **tab** key and your **up/down** arrow keys. Tab completion will allow you to enter in part of a filename or directory name and then it'll be completed it for you. Your up/down arrow keys will allow you to scroll through previous commands.

Now try navigating around on your own! See the animation below for some help.

![](/assets/CLI01.gif)

