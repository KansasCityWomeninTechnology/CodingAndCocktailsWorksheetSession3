1. Let's try running the previous command again. Press the up arrow to see your last command. Continue to press the up arrow to continue to see your previous commands. Press `Enter` when you find a command you want to run again. 
   {% hint style='info' %}
The up and down arrow traverse through your command history.
   {% endhint %}

1. We can also use `!!` to repeat the last command. Type `!!` <i class="fa fa-share fa-rotate-180"></i>.
 
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
Windows users- exit `bash` by typing `exit` <i class="fa fa-share fa-rotate-180"></i>. Cmder wraps **bash** functionality so Windows users can tap into **bash** when needed to mimic a more Linux OS like experience, but it isn't a full featured. Cmder can also use **bash** directly as a separate shell. The homework has a special Windows users only exercise using Cmder's bash shell.
   {% endhint %}

1. With the help of history view, we can use `!` operator with a number to repeat the nth command. Type `!-2` <i class="fa fa-share fa-rotate-180"></i> to repeat the second command at the bottom of your history. Type `!7` to repeat the seventh command at the top of your history.

1. To clear your terminal, type `clear` <i class="fa fa-share fa-rotate-180"></i>. The terminal looks so clean!

1. Make your computer talk to you. 
   {% tabs first="Macs", second="Windows", third="Chromebooks" %}

    {% content "first" %}
1. Type the following command `say "Coding and Cocktails is my favorite place"` <i class="fa fa-share fa-rotate-180"></i>.

1. You can add new voices under System Preferences -> Accessibility -> Speech. If you want to specify a voice, use the syntax  `say -v "Vicki" "hey there pardner"`.


    {% content "second" %}
This is an example where Cmder or **BASH** doesn't have the same utility. For Windows, we can use Powershell.

1. In the Windows task bar, search for "PowerShell". Open "Windows PowerShell Desktop App". 

1. Type the following command and press `Enter`.
```
PowerShell -Command "Add-Type –AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('Coding and Cocktails is my favorite place');"
```

    {% content "third" %}
Sorry Chromebook users, the online terminal doesn't have this capability.

    {% endtabs %}

