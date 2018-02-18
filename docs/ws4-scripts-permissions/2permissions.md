1. First view the current permissions on your script by typing `ls -l CnCScript.sh`.  You'll see `-rw-r--r--` as the current permissions.
    {% hint style='info' %}
Windows users will see `-rwxr-xr-x`. You don't need to change permissions on the file but we will walk through the exercise.
    {% endhint %}

1. Enter `chmod u+rwx CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i> into your command line prompt to grant execute permissions.

1. Now check permissions again by pushing the up arrow twice to scroll back through your commands back to `ls -l CnCScript.sh` and then press enter. You'll see that now the owner has execute (**x**) permission as well. 

1. Run the script by typing the following command for your OS and press `Enter`. 
   {% codetabs name="Mac", type="bash" -%} 
   ./CnCScript.sh
   {%- language name="Windows", type="bash" -%} 
   sh CnCScript.sh
   {%- language name="Chromebooks", type="bash" -%} 
   ./CnCScript.sh
   {%- endcodetabs %}


