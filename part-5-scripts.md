# Part 5: Scripts & Permissions

---

#### Shebangs!

Along with the command prompt, **scripts** can also be written as programs to be interpreted by the shell. For the most part, almost anything you can run at the command prompt, you can also include in a script, though there might sometimes be slight deviations in syntax.

To create a script, you'll need to write it and give it the proper **permissions** so that the shell can execute it. Permissions allow you to specify what users or groups can **read**, **write**, and/or **execute** a file.

So let's try it!

1. Open a new file in your CodingandCocktails folder by typing `vim CnCScript.sh`. This command will both create and open the file for you.
    {% hint style='info' %}
The '.sh' is optional but makes it easy for you to tell which files are scripts.
    {% endhint %}

2. Enter the following in your script. Remember, you'll type `i` to enter INSERT mode in vim. If you'd like to add more comments such as an author or date to your script, you can do that by starting the comment line with `#`.

    ```
    #!/bin/bash
    # My first script

    echo "Hello Coding & Cocktails!"
    ```
    {% hint style='info' %}
The `#!` is known as a **shebang** and tells the shell what **interpreter** to use. An interpreter is basically a program that executes commands. In this script, we're assigning the Bash shell as the interpreter. The rest of the script, in this case, then needs to be written in the Bash language. If you want to learn more about Bash, you can check out this Wikipedia entry: [https://en.wikipedia.org/wiki/Bash_(Unix_shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell)).
    {% endhint %}

3. Save your script within vim by typing `:wq`.

4. Enter`ls -alh` in the command line. Remember, you could also run `la` instead if you wanted to use the alias that was created earlier.
    {% hint style='info' %}
You'll see the permissions for each file listed in the left-most column. The third and fourth columns list the user and group ownership respectively. We won't have to change the ownership of the file \(which can be done with `chown`\) since our user will both be creating the file and running it.
    {% endhint %}

  Your shell uses **r**, **w**, and **x **along with corresponding numerical values **4**, **2**, and **1** for each to represent read, write, or execute. You'll need to specify values for the **owner **\(**u**\), \(**g**\)**roup**, and \(**o**\)**ther** in that order. We can run the following to add read, write, AND execute permissions for the owner.

5. Enter `chmod u+rwx CnCScript.sh` or `chmod 700 CnCScript.sh` into your command line prompt.
    {% hint style='info' %}
To get the numerical value for read, write, and execute, you add their individual values. So, 4+2+1=7. The first number denotes the permissions for the user while the second and third are for the group and other. "Other" refers to everyone else that's not a member of the owning group.
    {% endhint %}

6. Type in `./CnCScript.sh` and hit enter to run your script.

You've just written your first script! Congrats!
