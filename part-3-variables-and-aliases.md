# Part 3: Variables & Aliases

---

#### Creating Variables and Aliases

Variables can be created with the `export` command. Several programs and utilities use built in variables programmatically. Here's how to create and also how to display variable values:

1. Type `export MY_FAV=Greyhound`. Feel free to put in any value you'd like!
   * Be careful when including spaces - in that case, you'll want to enclose your value in quotation marks so it doesn't break up the command, i.e. `export MY_FAV="Moscow Mule"`.
2. Enter `echo $MY_FAV` in your command line. 
   * Note the `$` at the beginning of the variable.

Now try displaying the values for the built-in OS variables of HOME, USERNAME, and HOST. Remember, you should use the syntax `echo $VAR`.

**PATH** is a unique variable. It includes the locations of all executables. When you run a command, your shell looks in the directories specified there for an executable with a matching name. You can add a custom directories depending on where a program gets installed. Let's check out what's included in our path:

1. `echo $PATH`

To add directories to the PATH, you would use the syntax `export PATH=/some/directory:$PATH`. Notice that you can reference the PATH variable in creating the new PATH. Many installers do this step automagically for you!

So what's an alias? Basically, it's a shortcut you create to a command. For example, remember the `ls -al` command we used earlier? It gives us more information and makes the output easier to read. Let's bind it to `ls` to save us some keystrokes:

1. `alias ls="ls -al"`

Now you can enter `ls` and get the output for `ls -al` instead. You can imagine how much time this customization can save!

If you close out of your terminal and open a new one, you'll notice that the alias we just create didn't persist. That's because every time you open a new terminal, it's settings, namely what's called your **profile,** are reloaded. You can edit your profile by following these steps:

1. Create the file by typing `touch ~/.bash_profile`.
   * If the file already exists, its timestamp will be updated but no harm will be done.
2. Type `vim ~/.bash_profile` and hit enter. Then add the alias command we used above using INSERT mode with `i`.
   * Jump back to [**Part 1**](/part-1-navigation-and-basics.md) if you need some help with navigating in vim.
3. Type`source ~/.bash_profile` in your command line.
   * This will reload your settings.

You can watch the same steps from above in the following animation.

