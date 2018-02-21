  Now, close out of your terminal and open a new one. You'll notice that the alias we just create didn't persist. That's because every time you open a new terminal, its settings, namely what's called your **profile,** are reloaded.

You can edit your profile by following these steps:

1. Create the file by typing `touch ~/.bash_profile` ![](images/enter.png).
    {% hint style='info' %}
If the file already exists, its timestamp will be updated but no harm will be done.
    {% endhint %}

2. Type `vim ~/.bash_profile` ![](images/enter.png). Then add the alias command we used above using INSERT mode with `i`.
    {% hint style='tip' %}
Jump back to [**Part 1**](/part-1-navigation-and-basics.md) if you need some help with navigating in vim.
    {% endhint %}
    {% hint style='info' %}
Your custom variables, like the $MY_FAV_DRINK we set above, will also be lost when you close your terminal. You can add custom variables to your ~/.bash_profile as well by adding the `export MY_FAV_DRINK=Greyhound` command, for example, in its own line.
    {% endhint %}

3. Type`source ~/.bash_profile` ![](images/enter.png) in your command line. This will load or reload your profile settings.