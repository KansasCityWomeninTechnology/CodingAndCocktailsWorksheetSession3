1. We've made quite a few changes. We can see the history in the command line. Type `git log` <i class="fa fa-share fa-rotate-180"></i> to see all the changes you made tonight. It should looks similar to this

   ![](images/git-log.png)

   If we mapped out your commits, your git graph currently looks like this
   
   ![](images/git-graph-pre-squash.png)

   {% hint style='info' %}
   JAD TODO Fix
It shows each commit (with the unique identifier) and the commit message along with the author and date. Notice the top commit also has `(HEAD -> master)`. This says your own local copy of the "master" branch is at the top commit. Notice the bottom commit has `(origin/master, origin/HEAD)`. This is the last change that your remote, GitHub, is aware of. Your terminal may not show where HEAD is.
   {% endhint %}
      {% hint style='tip' %}
Your terminal automatically shows the output using 'less'. To exit out of 'less' type `q`.
   {% endhint %}

1. In the terminal type `git push` <i class="fa fa-share fa-rotate-180"></i> to push our changes to GitHub. That way other people can see our work. Oh oh! We got an error
   ```
**[terminal]
**[prompt LadyDev@Coding&Cocktails]**[path  ~/CodingAndCocktails/VersionControl/MyFirstRepo (cocktails-branch)]
**[delimiter λ ]**[command git push]
fatal: The current branch cocktails-branch has no upstream branch.
To push the current branch and set the remote as upstream, use
    git push --set-upstream origin cocktails-branch
   ```
   {% hint style='info' %}
The remote, GitHub, has no knowledge of 'cocktails-branch'. We need to provide the branch name (cocktails-branch) and where to create the branch (origin). We add the flag '--set-upstream' so that the remote has this branch reference and we don't have to provide the 'cocktails-branch' and 'origin' parameters for subsequent `git push` commands.
   {% endhint %}

1. Follow the instructions in the error and type `git push --set-upstream origin cocktails-branch` <i class="fa fa-share fa-rotate-180"></i>.

1. Type `git log --graph` <i class="fa fa-share fa-rotate-180"></i>. You should see your change on 'cocktails-branch' and the second commit from the top is where 'master' is. You diverged from 'master'. Your git graph looks like this

   ![](images/git-graph-branch.png)

   {% hint style='tip' %}
Use `q` to exit `less`.
   {% endhint %}


1. In Chrome, navigate to your "MyFirstRepo" page and reload the page. You should see your new file _cocktails.txt_. You can click on the file to see the contents.

1. You will also see **<span class="octicon octicon-history"></span> 2 commits** above the dropdown for 'master' branch. Click on it to navigate to your commit history. The commit history and path should match what you saw in the terminal.
