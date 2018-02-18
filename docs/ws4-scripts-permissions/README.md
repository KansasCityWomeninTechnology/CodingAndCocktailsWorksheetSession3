# Scripts & Permissions {#top}

{% hint style='tip' %}
While following along with the worksheet, type out the commands instead of doing a copy & paste unless explicitly stated to avoid inadvertently using any wrong characters.
{% endhint %}

<!-- trick markdown to give me a little space between these two sections of text -->
## 

This section will help guide you through the following steps:

{% include "./instruction-steps.html" %}


## Create shell scripts {#scripts} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Along with the command prompt, **scripts** are also used. Scripts are programs interpreted by the shell to handle more complex needs. You can script almost anything you can run at the command prompt though there might sometimes be slight deviations in syntax.

To create a script, you'll need to write it and give it the proper **permissions** so that the shell can execute it. Permissions allow you to specify what users or groups can **read**, **write**, and/or **execute** a file.

{% include "./1scripts.md" %}

## Editing file permissions {#permissions} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Your shell uses **r**, **w**, and **x** to represent **r**ead, **w**rite, or e**x**ecute. Specify values for the **owner (u)**, **(g)roup**, and **(o)ther** in that order. Scripts require proper permissions to run. We can use `chmod` to add read, write, AND execute permissions for the owner.
{% include "./2permissions.md" %}


<!-- trick markdown to give me a little space between these two sections of text -->
## 


## References and helpful links <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
[GNU/Linux Command-Line Summary for file permissions](https://linux.die.net/Linux-CLI/file-permissions.html)



