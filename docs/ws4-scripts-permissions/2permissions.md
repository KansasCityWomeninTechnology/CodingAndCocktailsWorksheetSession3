1. First view the current permissions on your script by typing `ls -l CnCScript.sh`.  You'll see `-rw-r--r--` as the current permissions.
    {% hint style='info' %}
Windows users will see `-rwxr-xr-x`. You don't need to change permissions on the file but we will walk through the exercise.
    {% endhint %}

1. Enter `chmod u+rwx CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i> into your command line prompt to grant execute permissions.

1. Now check permissions again by pushing the up arrow twice to scroll back through your commands back to `ls -l CnCScript.sh` and then press `Enter`. You'll see that now the owner has execute (**x**) permission as well. 

1. Run the script by typing `./CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i>.


   {% tabs first="Macs", second="Windows", third="Chromebooks" %}

    {% content "first" %}
1. Run the script by typing `./CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i>.

    {% content "second" %}
1. Run the script by typing `./CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i>.

    {% content "third" %}
1. Run the script by typing `sh CnCScript.sh` <i class="fa fa-share fa-rotate-180"></i>.
    {% endtabs %}
