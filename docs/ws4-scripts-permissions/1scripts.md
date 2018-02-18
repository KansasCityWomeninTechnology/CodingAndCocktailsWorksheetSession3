1. Navigate to your "CommandLineBasics" folder and create a new file there by typing `vim CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i>. This command will both create and open the file for you.
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
The `#!` is also known as a **shebang** and tells the shell what **interpreter** to use. An interpreter is basically a program that executes commands. In this script, we're assigning the Bash shell as the interpreter. The rest of the script, in this case, then needs to use the Bash language. If you want to learn more about Bash, you can check out this Wikipedia entry: [https://en.wikipedia.org/wiki/Bash_(Unix_shell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell)).
    {% endhint %}

3. Save your script within vim by first pressing the `Esc` key on your keyboard to exit insert mode and then typing `:wq` <i class="fa fa-share fa-rotate-180"></i>.

4. Enter `ls -alh` <i class="fa fa-share fa-rotate-180"></i> in the command line to see your script. You could also run `la` instead if you wanted to use the alias you created earlier and didn't delete it.
    {% hint style='info' %}
You'll see the permissions for each file listed in the left-most column. The third and fourth columns list the user and group ownership, respectively. We won't have to change the ownership of the file (using the `chown` command) since our user will both be creating the file and running it.
    {% endhint %}