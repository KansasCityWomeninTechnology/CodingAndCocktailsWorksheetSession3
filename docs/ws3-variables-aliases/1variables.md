1. Create a session variable by typing `export MY_FAV_DRINK=Greyhound` <i class="fa fa-share fa-rotate-180"></i>. You can use any value for your favorite drink you wish.
    {% hint style='info' %}
Be careful when including spaces - in that case, you'll want to enclose your value in quotation marks so it doesn't break up the command, i.e. `export MY_FAV_DRINK="Old Fashioned"`.
    {% endhint %}

1. To `echo` the variable, type `echo $MY_FAV_DRINK` <i class="fa fa-share fa-rotate-180"></i>.
   {% hint style='info' %}
We created session variables which means the variables are only available for the session. Try closing your terminal, reopening, and `echo` your variable.
   {% endhint %}

1. Now try displaying the values for the built-in OS variables of HOME and USERNAME by typing in the following command for your OS then press `Enter`.
  {% codetabs name="Mac", type="bash" -%} 
   echo $VAR
   {%- language name="Windows", type="bash" -%} 
   export
   {%- language name="Chromebooks", type="bash" -%} 
   export
   {%- endcodetabs %}

1. There's a special variable called the **PATH** variable. Let's see what's in it. Type `echo $PATH` <i class="fa fa-share fa-rotate-180"></i>.
   {% hint style='info' %}
It includes the locations of all executables, which are files or programs run by your computer. When you run a command, your shell looks in the directories specified there for an executable with a matching name. Most installers modify your path automatically for you to include any new paths needed!

You can append to **PATH** if you need, but we won't cover it here. You can also append to the **PATH** just for the session.
   {% endhint %}

   {% hint style='danger' %}
Be **VERY** careful editing your **PATH** as you could lose access to your programs!
   {% endhint %}
