1. Now we can commit our new file to git. Type `git commit -m "important file"` <i class="fa fa-share fa-rotate-180"></i>. You should see something like this in your terminal
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git commit -m "important file"]
[cocktails-branch dc2c473] important file
1 file changed, 1 insertion(+)
create mode 100644 cocktails.txt
   ```
  {% hint style='info' %}
We committed a snapshot of the files to the repository history. We see each of these commits in the git graph. The '-m' flag allows you to provide a description of the changes and is short for "message". This is important information for those who may collaborate on the code later.
   {% endhint %}
   {% hint style='tip' %}
If you accidentally hit `Enter` after you typed `git commit`, have no fear.

Your default text editor (default is vi) will open, where you can add your commit message. We'll cover vi later in the session so for now, grab a mentor for help!
   {% endhint %}

1. Your terminal changed back to how it looked before we added the _cocktails.txt_ file. Take a look at your git status and in GitKraken. 
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/session3/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git status]
On branch cocktails-branch
nothing to commit, working tree clean
   ```
1. We're building our own Git graph. You see 2 commits in GitKraken. We can view this in the terminal by typing `git log` <i class="fa fa-share fa-rotate-180"></i>. You'll see 2 commits in the terminal that matches up to what you see in GitKraken. A visualization of our initial commit and a new commit on a branch looks like this
   
   ![](images/git-graph.png)