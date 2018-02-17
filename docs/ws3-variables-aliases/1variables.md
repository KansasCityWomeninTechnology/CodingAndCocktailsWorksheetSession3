1. Create a session variable by typing the following command for your operating system. You can use any value for your favorite drink you wish.
   {% codetabs name="Mac", type="bash" -%} 
   export MY_FAV_DRINK=Greyhound
   {%- language name="Windows", type="bash" -%} 
   set MY_FAV_DRINK=Greyhound
   {%- language name="Chromebooks", type="bash" -%} 
   export MY_FAV_DRINK=Greyhound
   {%- endcodetabs %}

    {% hint style='info' %}
Be careful when including spaces - in that case, you'll want to enclose your value in quotation marks so it doesn't break up the command, i.e. `export MY_FAV_DRINK="Horsefeather"`.
    {% endhint %}

1. To `echo` the variable, type the following command for your operating system.
   {% codetabs name="Mac", type="bash" -%} 
   echo $MY_FAV_DRINK
   {%- language name="Windows", type="bash" -%} 
   echo %MY_FAV_DRINK%
   {%- language name="Chromebooks", type="bash" -%} 
   echo $MY_FAV_DRINK
   {%- endcodetabs %}

1. Now try displaying the values for the built-in OS variables of HOME and USERNAME by typing in the following command for your operating system. Remember, you should use the syntax `echo $VAR`.
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
