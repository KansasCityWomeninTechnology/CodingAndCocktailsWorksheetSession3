# Scripts & Permissions {#top}

{% hint style='tip' %}
While following along with the worksheet, type out the commands instead of doing a copy & paste to avoid inadvertently using any wrong characters.
{% endhint %}

<!-- trick markdown to give me a little space between these two sections of text -->
## 

This section will help guide you through the following steps:

{% include "./instruction-steps.html" %}


## Create shell scripts {#scripts} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
JAD TODO Text here?
Along with the command prompt, **scripts** can also be written as programs to be interpreted by the shell. For the most part, almost anything you can run at the command prompt, you can also include in a script, though there might sometimes be slight deviations in syntax.

To create a script, you'll need to write it and give it the proper **permissions** so that the shell can execute it. Permissions allow you to specify what users or groups can **read**, **write**, and/or **execute** a file.

{% include "./1scripts.md" %}

## Editing file permissions {#permissions} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
JAD TODO Text here?
  Your shell uses **r**, **w**, and **x **along with corresponding numerical values **4**, **2**, and **1** for each to represent read, write, or execute. You'll need to specify values for the **owner **\(**u**\), \(**g**\)**roup**, and \(**o**\)**ther** in that order. Scripts require proper permissions in order to be ran. We can use `chmod` to add read, write, AND execute permissions for the owner.
{% include "./2permissions.md" %}

<!-- trick markdown to give me a little space between these two sections of text -->
## 

## Checkpoint <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Compare your _styles.css_ against the answer key for your work so far. It might look a little different depending on the color palette you chose.  


<!-- trick markdown to give me a little space between these two sections of text -->
## 


## References and helpful links <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
[Mozilla Developer Network CSS reference documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)



