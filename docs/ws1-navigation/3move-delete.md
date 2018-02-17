1. Type `cp CLIFun.txt CLIFun2.txt` <i class="fa fa-share fa-rotate-180"></i>. Do you see the new file in the explorer?
      {% hint style='info' %}
If you do an `ls -al` you'll see there's now a **CLIFun2.txt** file with the same size as the **CLIFun.txt** file but with a more current timestamp.
      {% endhint %}

1. Let's remove "CLIFun2.txt" by typing `rm CLIFun2.txt` <i class="fa fa-share fa-rotate-180"></i>. 

1. Now that we know how to copy files, let's try copying a directory as well. Change directory to "CodingAndCocktails" then type `cp CommandLineBasics CommandLineBasics2` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='info' %}
Oh no, we got an error! It looks like `cp` doesn't work with directories, but we can copy a directory by adding an option to `cp`. We'll add a **-r** for **r**ecursive.
      {% endhint %}

1. Let's try that again. Type `cp -r CommandLineBasics CommandLineBasics2` <i class="fa fa-share fa-rotate-180"></i>. 
      {% hint style='tip' %}
Don't forget your tab completion!
      {% endhint %}

1. List the directory contents to make sure the copy worked by entering `ls -al` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='tip' %}
This time, you'll see a **CommandLineBasics2** directory that's the same as the directory we copied it from, except that it has a more current timestamp. You can also check it out in the explorer.
      {% endhint %}

1. To remove the directory, use the recursive option again by typing `rm -r CommandLineBasics2` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='danger' %}
Be **VERY** careful when running rm commands. If you do it from the wrong directory, you could potentially remove your entire **OS** \(**O**perating **S**ystem, i.e. Windows or Mac OSx\) or other really important data!!
      {% endhint %}

1. Now let's move files. Navigate to the "CodingAndCocktails" directory and type `mv CommandLineBasics/CLIFun.txt .` <i class="fa fa-share fa-rotate-180"></i>.
      {% hint style='tip' %}
Remember, **.** is a shortcut for the current directory.
      {% endhint %}
