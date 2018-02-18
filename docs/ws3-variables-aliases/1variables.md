1. Create a session variable by typing the following command for your OS and pressing `Enter`. You can use any value for your favorite drink you wish.
   {% codetabs name="Mac", type="bash" -%} 
   export MY_FAV_DRINK=Greyhound
   {%- language name="Windows", type="bash" -%} 
   set MY_FAV_DRINK=Greyhound
   {%- language name="Chromebooks", type="bash" -%} 
   export MY_FAV_DRINK=Greyhound
   {%- endcodetabs %}

    {% hint style='info' %}
Be careful when including spaces - in that case, you'll want to enclose your value in quotation marks so it doesn't break up the command, i.e. `export MY_FAV_DRINK="Old Fashioned"`.
    {% endhint %}

1. To `echo` the variable, type the following command for your OS and press `Enter`.
   {% codetabs name="Mac", type="bash" -%} 
   echo $MY_FAV_DRINK
   {%- language name="Windows", type="bash" -%} 
   echo %MY_FAV_DRINK%
   {%- language name="Chromebooks", type="bash" -%} 
   echo $MY_FAV_DRINK
   {%- endcodetabs %}

1. Now try displaying the values for the built-in OS variables of HOME and USERNAME by typing in the following command for your OS then press `Enter`.
  {% codetabs name="Mac", type="bash" -%} 
   echo $VAR
   {%- language name="Windows", type="bash" -%} 
   set
   {%- language name="Chromebooks", type="bash" -%} 
   echo $VAR
   {%- endcodetabs %}

   {% hint style='working' %}
We created session variables which means the variables are only available for the session. Try closing your terminal, reopening, and `echo` your variable.
   {% endhint %}

1. There's a special variable called the PATH variable. Let's see what's in it. Type the following command for your OS and press `Enter`.
  {% codetabs name="Mac", type="bash" -%} 
   echo $PATH
   {%- language name="Windows", type="bash" -%} 
   echo %PATH%
   {%- language name="Chromebooks", type="bash" -%} 
   echo $PATH
   {%- endcodetabs %}

   {% hint style='info' %}
It includes the locations of all executables, which are files or programs run by your computer. When you run a command, your shell looks in the directories specified there for an executable with a matching name. Most installers modify your path automatically for you to include any new paths needed!

You can append to PATH if you need, but we won't cover it here. You can also append to the PATH just for the session.
   {% endhint %}

   {% hint style='danger' %}
Be **VERY** careful editing your PATH as you could lose access to your programs!
   {% endhint %}
