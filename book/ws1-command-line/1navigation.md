{% hint style='info' %}
The <i class="fa fa-share fa-rotate-180"></i> icon tells you when to press `Enter`.
{% endhint %}

1. Open a terminal for your OS. For Windows, open Cmder. For Macs, open iTerm2.

1. In your terminal, type `pwd` <i class="fa fa-share fa-rotate-180"></i> in your CLI to see your current directory. `pwd` stands for **p**rint **w**orking **d**irectory. 
   {% hint style='info' %}
You should be in your home directory. For Macs, you should see `~` after your prompt. For Windows, you should see `C:\Users\<Your user name>` above the lambda (**λ**). We will refer to this directory as your home directory in the remainder of the worksheet.
    {% endhint %}

1. Open a file explorer by using the following command for your operating system (select the tab for your operating system)
    {% codetabs name="Mac", type="bash" -%} 
    open .
    {%- language name="Windows", type="bash" -%} 
    start .
    {%- endcodetabs %}

    {% hint style='tip' %}
Being able to visualize your work will help reinforce concepts. View the worksheet, terminal, and file explorer for the command line section of the worksheet all at the same time by adjusting application layout. 

We want to lay out our workspace to look like this.

![](images/desktop.png)

For Windows users, use `windows key` + `left arrow` or `windows` + `right arrow` to resize the application and position to the left or right half of your screen.

For Mac users, hold down the full-screen button in the upper-left corner of a window to shrink and position to the left or right side of the screen. Release the button, then click another window to begin using both windows side by side.

Mentors are happy to help!
   {% endhint %}
 
1. In the terminal, type `ls` <i class="fa fa-share fa-rotate-180"></i> to see the contents of your current directory. You should see the same files in the terminal as you see in the explorer.

1. Next, **c**hange **d**irectory into the "CodingAndCocktails" directory listed in the output of `ls` by typing `cd CodingAndCocktails` <i class="fa fa-share fa-rotate-180"></i>. Navigate to your "CodingAndCocktails" directory in the file explorer.
   {% hint style='danger' %}
If you don't have a "CodingAndCocktails" directory, take a moment to [set up your workspace](/setup).
   {% endhint %} 
   {% hint style='tip' %}
Both Cmder and oh-my-zsh use formatting to distinguish between what's a directory and what's a file. You won't be able to `cd` into a file.
   {% endhint %}

1. In the "CodingAndCocktails" directory, type `ls` <i class="fa fa-share fa-rotate-180"></i> again to see what's listed there. You should see the same files and folders from the output of `ls` in the file explorer.

1. Type `ls -al` <i class="fa fa-share fa-rotate-180"></i> and compare it to your previous output.  You should see more information and all files, including hidden files.
  {% hint style='info' %}
A hidden file is something that isn't normally visible. Examples are files prefixed with `.`, such as profile files. We'll learn more about profile files later in the worksheet. You'll also see `.` and `..`. These are special files representing your current directory and parent directory.
   {% endhint %}

1. Let's move back up one directory-- the parent directory of "CodingAndCocktails". To do this, type `cd ..` <i class="fa fa-share fa-rotate-180"></i>.
    {% hint style='info' %}
The `..` is a shortcut for the parent directory. A parent directory would be the directory that contains your current directory. No matter where you are, `cd ..` is always a valid command.
    {% endhint %}
