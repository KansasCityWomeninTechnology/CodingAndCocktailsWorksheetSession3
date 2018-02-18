1. Let's create an alias. Type the following command for your OS and press `Enter`.
   {% codetabs name="Mac", type="bash" -%} 
   alias la="ls -alh"
   {%- language name="Windows", type="bash" -%} 
   alias la=ls -alh
   {%- language name="Chromebooks", type="bash" -%} 
   alias la="ls -alh"
   {%- endcodetabs %}

1. Type `la` <i class="fa fa-share fa-rotate-180"></i> and get the output for `ls -alh` instead. You can imagine how much time customization like this can save!
   {% hint style='info' %}
The alias we created is not persistent for Mac and Chromebook users.
Windows users- The alias we created is persistent because Cmder automatically saves it for us.
   {% endhint %}

1. We can see all the aliases available to us (including the one we created) by typing `alias` <i class="fa fa-share fa-rotate-180"></i>.

1. We can remove the `la` alias by typing `unalias la` <i class="fa fa-share fa-rotate-180"></i>.

1. Inspect all aliases available to see if the `la` alias still exists.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>alias</code> <i class="fa fa-share fa-rotate-180"></i>. <code>la</code> should no longer be.
</details>
   {% endhint %}