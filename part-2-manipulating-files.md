# Part 2: Manipulating Files

---

#### Create and Edit Files and Directories

Let's get straight to learning how to manipulate files and directory structures!

1. Change into your home folder by typing `cd ~`. Type `ls -al` to check if a **CodingAndCocktails** folder already exists.

2. In your CodingAndCocktails folder, create a **CommandLineBasics** folder by entering in `mkdir CommandLineBasics`.

3. Then change into your newly created directory by typing `cd CommandLineBasics`.

4. Let's create a file by typing `touch CLIFun.txt`.
    {% hint style='info' %}
If you go to that same location through your GUI like you might be used to, you'll see the file created there as a visual representation. You open the current directory you're in on a Mac by typing `open .`. On a Windows machine, `start .` will do the same.
    {% endhint %}

5. Now, we'll want to add some content to your file. Open your file in vim by typing `vim CLIFun.txt`.
    {% hint style='info' %}
While **vim** is one option for a text editor, there are many others available. You can use this [**vim cheat sheet**](https://vim.rtorr.com/)** **to take full advantage of** **its powerful features.
    {% endhint %}

   What's with all the squigglies?!?

   ![](/images/vim_squigglies.png)

   Don't worry! By learning a few basic vim commands, you'll be saving contents in your files in no time. Let's start by copying the [**lorem ipsum**](https://en.wikipedia.org/wiki/Lorem_ipsum) text below.

    ```
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
      et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
      aliquip ex ea commodo consequat.
      ```
6. Go back to iTerm2/Git Bash and hit `i`. That'll put you into **INSERT** mode.

7. Now hit **⌘V** on your Mac or **Shift + Ins** in Git Bash on your Windows laptop to paste the text you copied.

8. Hit `esc` to exit out of **INSERT** mode.

9. Next, type in `:wq` and then hit **Enter**. Awesome, now we've got some content to play with!
    {% hint style='info' %}
The 'w' stands for **write** and the 'q' stands for **quit**.
    {% endhint %}

10. Now type `cat CLIFun.txt` to display the contents of the file. Cool!

11. To add more content, type `vim CLIFun.txt` to enter the editor again. Hit `i` again like we did before and start entering in some text.

   But that messed up our lorem ipsum sample! What to do?!? No worries, let's just close out of the text editor without saving our changes. We did a 'write' and then 'quit' earlier, let's instead skip the 'write' part.

12. Hit `esc` again to exit out of **INSERT** mode.

13. Hit `:q` then **Enter**.
      {% hint style='info' %}
You'll be prompted with '**E37: No write since last change \(add ! to override\)**'. Follow the instructions there. Hit `:q!` then **Enter**.
      {% endhint %}

14. Type `cat CLIFun.txt` again to confirm your changes weren't saved.

   Let's now work with `cp` and `rm`** **to make copies of our file and remove files.

15. Type `cp CLIFun.txt CLIFun2.txt`.
      {% hint style='info' %}
If you do an `ls -al` you'll see there's now a **CLIFun2.txt** file with the same size as the **CLIFun.txt** file but a more current timestamp.
      {% endhint %}

16. Ok, let's undo that by entering `rm CLIFun2.txt`.

   Let's try copying a directory as well.

17. Type `cp CommandLineBasics CommandLineBasics2` after changing into the CodingAndCocktails parent directory.
      {% hint style='info' %}
Oh no, we got an error again: '**cp: CommandLineBasics is a directory \(not copied\)**'! It looks like `cp` doesn't work with directories, but actually, we can copy a directory by adding an option to `cp`. We'll add a **-r** for **recursive**.
      {% endhint %}

18. Let's try that again. Type `cp -r CommandLineBasics CommandLineBasics2`.
      {% hint style='tip' %}
Don't forget your tab completion! This time, you'll see a **CommandLineBasics2** directory that's the same as the directory we copied it from, except that it has a more current timestamp.
      {% endhint %}

19. To remove the directory, use the recursive option again by typing `rm -r CommandLineBasics2`.
      {% hint style='danger' %}
Be **VERY** careful when running rm commands. If you do it from  the wrong directory, you could potentially remove your entire **OS** \(**O**perating **S**ystem, i.e. Windows or Mac OSx\) or other really important data!!
      {% endhint %}

   What if we need to move a file? Well, then use `mv`! The proper syntax for the command is `mv <source> <destination>`.

20. Type `mv ~/CodingAndCocktails/CommandLineBasics/CLIFun.txt ~/CodingAndCocktails/`.
      {% hint style='info' %}
If you're in the CodingAndCocktails directory, the command `mv CommandLineBasics/CLIFun.txt .` will also work. Remember, '**.**' is a shortcut for the current directory.
      {% endhint %}


Another command that's useful for files is `wc`. You can remember it as **word count**, and it'll be in the syntax `wc [options] filename`. Here are some available options you can try out:

![](/images/wc_options.png)

If you need further help with the `vim` command, check out the video below.

{% raw %}
  <video id="CLI_Part2" class="video-js" controls preload="auto" width="900" height="600"
  poster="CLI_Part2.jpg" data-setup="{}">
  <source src="videos/CLI_Part2.mp4" type='video/mp4'>
  <p class="vjs-no-js">
    To view this video please enable JavaScript, and consider upgrading to a web browser that
    <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a>
  </p>
  </video>
{% endraw %}
