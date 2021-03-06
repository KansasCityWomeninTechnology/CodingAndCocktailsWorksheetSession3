1. Let's create a new file by using the command line. Type `touch cocktails.txt` <i class="fa fa-share fa-rotate-180"></i>. 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command touch cocktails.txt]
   ```
   {% hint style='tip' %}
Your terminal may have changed when you created a new file. Mac users may see a yellow X appear and Cmder users may see the color of '(cocktails-branch)' branch name change. This is a way your terminal helps you keep track of changes in your git repository.
   {% endhint %}

1. Let's check out the git status again. This time the terminal lists _cocktails.txt_ as an untracked file.
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git status]
On branch cocktails-branch
Your branch is up to date with 'origin/cocktails-branch'.
Untracked files:
(use "git add <file>..." to include in what will be committed)
**[error    cocktails.txt]
nothing added to commit but untracked files present (use "git add" to track)
   ```
   {% hint style='info' %}
An untracked file is a file that Git doesn't know about. You have to explicitly ask Git to track a file. Git doesn't do this automatically in case you accidentally include files that shouldn't be in source control (such as large files or application files).
   {% endhint %}

1. We can add the file to Git and stage the file at the same time by typing `git add cocktails.txt` <i class="fa fa-share fa-rotate-180"></i>.

1. Let's check out the status again. This time the terminal lists _cocktails.txt_ as a change to be committed. 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git status]
On branch cocktails-branch
Your branch is up to date with 'origin/cocktails-branch'.
Changes to be committed:
(use "git reset HEAD <file>..." to unstage)
**[warning    new file:   cocktails.txt]
   ```

1. In GitKraken, click on the **View change** button or click on "//WIP" in the git tree view to see the staged files.

   ![](images/gitkraken-staged-files.png)

1. Oops! We meant to add some text to the file. It should say "My favorite cocktail is" in _cocktails.txt_. We need to fix that. Open _cocktails.txt_ in any editor you want to add the text. Make the change and save the file.

1. Check the git status in the terminal and take a look at GitKraken. Your terminal shows _cocktails.txt_ as unstaged and ready to be committed. What?! ![](../images/emojis/confused-face.png) 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git status]
On branch cocktails-branch
Your branch is up to date with 'origin/cocktails-branch'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)  
**[warning    new file:   cocktails.txt]
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
**[error     modified:   cocktails.txt]
   ```

   {% hint style='info' %}
This is because when you ran `git add`, Git staged the file in the state at that time. With a new change, we have to stage the file again.  
   {% endhint %}

   {% hint style='working' %}
In GitKraken, click on the _cocktails.txt_ in the **Staged Files** list at the bottom right of the application. Notice there's nothing to display in the diff view. Now click on _cocktails.txt_ in the **Unstaged Files** list at the top right of the application. We now see our text change.   
   {% endhint %}

1. Stage _cocktails.txt_.
   {% hint style='working' %}
<details>
<summary>
Need a little help? Expand this section for guidance. 
</summary>
Type <code>git add cocktails.txt</code> <i class="fa fa-share fa-rotate-180"></i>.
</details>
   {% endhint %}

