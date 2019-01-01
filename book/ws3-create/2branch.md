1. Let's create a branch for us to work in called 'cocktails-branch'. In the terminal, type `git checkout -b cocktails-branch` <i class="fa fa-share fa-rotate-180"></i>. It should look like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (master)]
**[delimiter λ ]**[command git checkout -b cocktails-branch]
Switched to a new branch 'cocktails-branch'
   ```
   {% hint style='info' %}
We passed in the '-b' flag into `git checkout` command. This means we'll create and checkout a branch at the same time.
   {% endhint %}
   {% hint style='tip' %}
Your terminal might look a little different after creating a branch. The terminals we have you use include the branch name, so you should see 'cocktails-branch' included in your prompt.
   {% endhint %}

1. Type `git status` <i class="fa fa-share fa-rotate-180"></i>. It should look something like this
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git status]
On branch cocktails-branch
nothing to commit, working tree clean

   ```