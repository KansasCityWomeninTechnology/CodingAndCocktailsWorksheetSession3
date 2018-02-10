   Let's now work with `cp` and `rm`** **to make copies of our file and remove files.

15. Type `cp CLIFun.txt CLIFun2.txt` ![](images/enter.png).
      {% hint style='info' %}
If you do an `ls -al` you'll see there's now a **CLIFun2.txt** file with the same size as the **CLIFun.txt** file but a more current timestamp.
      {% endhint %}

16. Ok, let's undo that by typing `rm CLIFun2.txt` ![](images/enter.png).

   Let's try copying a directory as well.

17. Change directory into the CodingAndCocktails parent directory then type `cp CommandLineBasics CommandLineBasics2` ![](images/enter.png).
      {% hint style='info' %}
Oh no, we got an error again: '**cp: CommandLineBasics is a directory \(not copied\)**'! It looks like `cp` doesn't work with directories, but actually, we can copy a directory by adding an option to `cp`. We'll add a **-r** for **recursive**.
      {% endhint %}

18. Let's try that again. Type `cp -r CommandLineBasics CommandLineBasics2` ![](images/enter.png).
      {% hint style='tip' %}
Don't forget your tab completion!
      {% endhint %}

19. List the directory contents to make sure the copy worked by entering `ls -al` ![](images/enter.png).
      {% hint style='tip' %}
This time, you'll see a **CommandLineBasics2** directory that's the same as the directory we copied it from, except that it has a more current timestamp.
      {% endhint %}

20. To remove the directory, use the recursive option again by typing `rm -r CommandLineBasics2` ![](images/enter.png).
      {% hint style='danger' %}
Be **VERY** careful when running rm commands. If you do it from  the wrong directory, you could potentially remove your entire **OS** \(**O**perating **S**ystem, i.e. Windows or Mac OSx\) or other really important data!!
      {% endhint %}

#### Moving a file or directory

What if we need to move a file? Well, we can use `mv`! The proper syntax for the command is `mv <source> <destination>`.

{% hint style='danger' %}
Chromebooks Only: Cloud9 users remember to use `~/workspace` in place of `~`
{% endhint %}

1. Type `mv ~/CodingAndCocktails/CommandLineBasics/CLIFun.txt ~/CodingAndCocktails/` ![](images/enter.png).
      {% hint style='info' %}
If you're in the CodingAndCocktails directory, the command `mv CommandLineBasics/CLIFun.txt .` will also work. Remember, **.** is a shortcut for the current directory.
      {% endhint %}

