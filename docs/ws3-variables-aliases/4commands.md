1. Let's try running the previous command again. Press the up arrow to see your last command. Continue to press the up arrow to continue to see your previous commands. Press `Enter` when you find a command you want to run again. 
   {% hint style='info' %}
The up and down arrow traverse through your command history.
   {% endhint %}

1. We can also use `!!` to repeat the last command. Type `!!` <i class="fa fa-share fa-rotate-180"></i>.
 
1. You can see your command history by typing `history` <i class="fa fa-share fa-rotate-180"></i>.

1. Your history has a lot and it scrolls off the terminal. What do we do if we want to inspect the history? We can redirect the output to file. And also we can pipe the output of `history` so it's more readable in the terminal by using `less`. Type `history | less` <i class="fa fa-share fa-rotate-180"></i>. 

1. Use the up and down arrow to scroll through the output. When you're finished looking, press `q` to quit.

1. With the help of history view, we can use `!` operator with a number to repeat the nth command. Type `!-2` <i class="fa fa-share fa-rotate-180"></i> to repeat the second command at the bottom of your history. Type `!7` to repeat the seventh command at the top of your history.

1. To clear your terminal, type `clear` <i class="fa fa-share fa-rotate-180"></i>. The terminal looks so clean!

1. Make your computer talk to you. 
   {% tabs first="Mac", second="Windows", third="Chromebook" %}

    {% content "first" %}
1. Type the following command `say "Coding and Cocktails is my favorite place"` <i class="fa fa-share fa-rotate-180"></i>.

1. You can add new voices under **System Preferences** -> **Accessibility** -> **Speech**. If you want to specify a voice, use the syntax  `say -v "Vicki" "hey there pardner"`.


    {% content "second" %}
This is an example where Cmder or **BASH** doesn't have the same utility. For Windows, we can use Powershell.

1. In Cmder, open a new tab using PowerShell as Admin. If you need guidance, take a look at [Using Cmder section](https://codingandcocktailskc.gitbooks.io/coding-cocktails-the-tools/content/tools-command-line/#using-cmder) in The Tools setup.

1. Copy the following command and paste into the terminal using `CTRL+v` <i class="fa fa-share fa-rotate-180"></i>.
```
PowerShell -Command "Add-Type –AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('Coding and Cocktails is my favorite place');"
```

    {% content "third" %}
Sorry Chromebook users, the online terminal doesn't have this capability.

    {% endtabs %}

