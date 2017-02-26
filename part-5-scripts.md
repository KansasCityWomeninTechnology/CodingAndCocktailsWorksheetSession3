# Part 5: Scripts & Permissions

---

#### Shebangs!

Along with the command prompt, **scripts** can also be written as programs to be interpreted by the shell. For the most part, almost anything you can run at the command prompt, you can also include in a script, though there might sometimes be slight deviations in syntax.

To create a script, you'll need to write it and give it the proper **permissions** so that the shell can execute it. Permissions allow you to specify what users or groups can **read**, **write**, and/or **execute** a file.

So let's try it!

1. Open a new file in your CodingandCocktails folder by typing `vim CnCScript.sh`.
   * the '.sh' is optional but makes it easy for you to tell what files are scripts
2. Enter the following in your script. Remember, you'll type `i` to enter INSERT mode in vim.

   * ```
     #!/bin/bash
     # My first script

     echo "Hello Coding & Cocktails!"
     ```

3. Save your script within vim by typing `:wq`.

When you enter`ls -al` in the command line, you'll see the permissions for each file listed in the left-most column. The third and fourth columns list the user and group ownership respectively. We won't have to change the ownership of the file \(which can be done with `chown`\) since our user will both be creating the file and running it.

Your shell uses **r**, **w**, and **x **along with corresponding numerical values **4**, **2**, and **1** for each to represent read, write, or execute. You'll need to specify values for the **owner **\(**u**\), \(**g**\)**roup**, and \(**o**\)**ther** in that order. We can run the following to add read, write, AND execute permissions for the owner.

1. Enter `chmod u+rwx CnCScript.sh` or `chmod 700 CnCScript.sh` into your command line prompt.
   * To get the numerical value for read, write, and execute, you add their individual values. So, 4+2+1=7. The first number denotes the permissions for the user while the second and third are for the group and other. "Other" refers to everyone else that's not an owner of a member of the owning group.
2. Type in `./CnCScript.sh` and hit enter to run your script.

You've just written your first script! Yay! If you need some visual help, check out the animation below.

