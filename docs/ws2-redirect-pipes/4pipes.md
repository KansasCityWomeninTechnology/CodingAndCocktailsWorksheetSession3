1. We can pipe output from one command to another and create powerful commands. Type `ls | grep .txt` <i class="fa fa-share fa-rotate-180"></i> to view all txt files in the current directory.
   {% hint style='info' %}
We are using the pipe operator (`|`) to take the output of `ls` and use it as input for `grep`.
   {% endhint %}

   Since we only have txt files this isn't too useful.

1. Type `ls | grep f` <i class="fa fa-share fa-rotate-180"></i>. Now we see 1 file __files.txt__ because it has a 'f' in the name.

1. Suppose we don't care about casing. Type `ls | grep -i f` <i class="fa fa-share fa-rotate-180"></i>. Now we see 2 files
   ![](./images/pipe.png)

   {% hint style='info' %}
The functionality of `|` seems similar to `>` or `>` but there is a distinction. Pipes (`|`) redirects data from one command to another command but redirection operators (`>` and `>>`) redirects the output of the command to file.
   {% endhint %}