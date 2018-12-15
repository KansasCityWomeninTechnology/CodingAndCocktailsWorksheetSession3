1. Type `cp CLIFun.txt CLIFun2.txt` <i class="fa fa-share fa-rotate-180"></i>. Do you see the new file in the explorer?
      {% hint style='info' %}
If you do an `ls -al` you'll see there's now a _CLIFun2.txt_ file with the same size as the _CLIFun.txt_ file but with a more current timestamp.
      {% endhint %}

1. Now that we know how to copy files, let's try copying a directory as well. Change directory to "CodingAndCocktails" then type `cp session3 session3-2` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='info' %}
Oh no, we got an error! It looks like `cp` doesn't work with directories, but we can copy a directory by adding an option to `cp`. We'll add a **-r** for **r**ecursive.
      {% endhint %}

1. Let's try that again. Type `cp -r session3 session3-2` <i class="fa fa-share fa-rotate-180"></i>. 
      {% hint style='tip' %}
Don't forget your tab completion!
      {% endhint %}

1. List the directory contents to make sure the copy worked by entering `ls -al` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='tip' %}
This time, you'll see a "session3-2" directory that's in the same as the directory we copied it from, except that it has a more current timestamp. You can also check it out in the explorer.
      {% endhint %}

1. To remove the directory, use the recursive option again by typing `rm -r session3-2` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='danger' %}
Be **VERY** careful when running rm commands. If you do it from the wrong directory, you could potentially remove your entire **OS** \(**O**perating **S**ystem, i.e. Windows or macOS\) or other really important data!!
      {% endhint %}

1. Now let's move files. Navigate to the "CodingAndCocktails" directory and type `mv session3/CLIFun.txt .` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='tip' %}
Remember, `.` is a shortcut for the current directory.
      {% endhint %}

1. Let's remove _CLIFun2.txt_ by typing `rm CLIFun2.txt` <i class="fa fa-share fa-rotate-180"></i>. 

1. There's a lot of commands in the terminal now and it looks a little cluttered. Let's clear it all out by using the `clear` command. Type `clear` <i class="fa fa-share fa-rotate-180"></i>.

1. Sometimes we need a reminder of all the different commands we used. We can use `history` command to help. Type `history <i class="fa fa-share fa-rotate-180"></i>.

1. Woah, that was a lot. Let's clear out the terminal using the up arrow. Press up arrow and you'll see your last command `history` appear after the prompt. Cool! Press up arrow again to see `clear`. Press `Enter` to run the command.
