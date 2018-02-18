1. Let's try running the previous command again. Press the up arrow to see your last command. Continue to press the up arrow to continue to see your previous command. Press `Enter` when you find a command you want to run again. 
   {% hint style='info' %}
The up and down arrow traverse through your command history.
   {% endhint %}

1. You can see your command history by typing `history` <i class="fa fa-share fa-rotate-180"></i>.

1. Your history has a lot and it scrolls off the terminal. What do we do if we want to inspect the history? We can redirect the output to file. And also we can pipe the output of `history` so it's more readable in the terminal by using `less`. Type the following command for your OS and press `Enter`. If your OS requires more than 1 command, press `Enter` between each. 
   {% codetabs name="Mac", type="bash" -%} 
   history | less
   {%- language name="Windows", type="bash" -%} 
   bash
history | less
   {%- language name="Chromebooks", type="bash" -%} 
   history | less
   {%- endcodetabs %}

   You can use the down arrow to scroll through the output. When you're finished looking, press `q` to quit.

   {% hint style='info' %}
Windows users- exit bash by typing `exit` <i class="fa fa-share fa-rotate-180"></i>.
   {% endhint %}

1. To clear your terminal, type `clear` <i class="fa fa-share fa-rotate-180"></i>. The terminal looks so clean!
