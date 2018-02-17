1. The `echo` command echos whatever we type but doesn't make any changes in the commandline. Type `echo Cocktail ladies are awesome` <i class="fa fa-share fa-rotate-180"></i>.

1. In the "CommandLineBasics" directory, we'll redirect output to a file by typing `echo first grab a cocktail > steps.txt` <i class="fa fa-share fa-rotate-180"></i>. Inspect the directory in the explorer. We now have a new file "steps.txt".
      {% hint style='info' %}
The `>` operator takes the output of `echo`, the first command, and redirects the output from the console to a file instead.
      {% endhint %}

1. Type `cat steps.txt` <i class="fa fa-share fa-rotate-180"></i> to read the content of the file. Open the file in the explorer to see the contents. 😎
      {% hint style='danger' %}
Don't forget to close the file so that we have access to write to it.
      {% endhint %}

1. Great! Let's add another step! Type `echo as people sit at your table, get to know them > steps.txt` <i class="fa fa-share fa-rotate-180"></i>. Read the content of the file using `cat` or by opening the file in the explorer. Uh oh! Where's the first step?
      {% hint style='info' %}
The `>` operator overwrites existing contents.
      {% endhint %}

1. It's not what we wanted but we can work with this. Rename "steps.txt" to "steps-temp.txt" by using the `mv` command. Type `mv steps.txt steps-temp.txt` <i class="fa fa-share fa-rotate-180"></i>. Inspect your directory using the explorer.

1. This time we'll use the `>>` operator. Type `echo first grab a cocktail >> steps.txt` <i class="fa fa-share fa-rotate-180"></i>. Inspect the file and contents using `ls` and `cat` operators.

1. Append the next step to the file by typing `echo then download any tools you need >> steps.txt` <i class="fa fa-share fa-rotate-180"></i>. Inspect the file and contents using the commandline or through the file explorer.

1. We can use `cat` to combine files. Let's append the contents of "steps-temp.txt" to "steps.txt" by typing `cat steps-temp.txt >> steps.txt` <i class="fa fa-share fa-rotate-180"></i>. Inspect the contents of "steps.txt" using the commandline or through the file explorer.

1. Combining those two file saved us from typing! We no longer need "steps-temp.txt" so delete using the `rm` command. 
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>rm steps-temp.txt</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

1. Let's try redirection with another command. You can list all the files in your directory by typing `ls > files.txt`. Inspect the file and contents using the commandline or through the file explorer.
