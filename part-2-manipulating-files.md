# Part 2: Manipulating Files

---

#### Create and Edit Files and Directories

Let's get straight to using the command line to learn how to manipulate files and directory structure!

1. Change into your home folder with `cd ~`. Use `ls -al` to check if a **CodingandCocktails** folder already exists.
2. If it doesn't, create it using `mkdir CodingandCocktails`. Note that the command line is **CASE-SENSITIVE**, so watch your capitalization!
3. In your CodingandCocktails folder, create a **CommandLineBasics** folder with `mkdir CommandLineBasics`.

4. Let's create a file! Do this by running `touch CLIFun`.

5. Now, we'll want to add some content to your file. We'll use **vim**, one option for a text editor. Open your file in vim using `vim CLIFun`.

6. What's with all the squigglies?!? Don't worry! By learning a few basic vim commands, you'll be saving contents in your files in no time. Let's start by copying the [**lorem ipsum**](https://en.wikipedia.org/wiki/Lorem_ipsum) text below.

7. ```
   Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
   et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut 
   aliquip ex ea commodo consequat.
   ```
8. Now that there's a good sample text in your clipboard, go back to iTerm2/Git Bash. There, hit `i`. That'll put you into **INSERT** mode. Now hit **⌘V** on your Mac or **CTRL + V** on your Windows laptop to paste the text you copied. Next, type in `:wq` and then hit **Enter**. The 'w' stands for **write** and the 'q' stands for **quit**. Awesome, now we've got some content to play with!

9. Now use `cat CLIFun` to display the contents of the file. Cool!

10. If you need to make further changes, just run `vim CLIFun` to enter the editor again. Let's do that and add some more content. Hit `i` again like we did before and start entering in some text.

11. But that messed up our lorem ipsum sample! What to do?!? No worries, let's just close out of the text editor without saving our changes. We did a 'write' and then 'quit' earlier, let's instead skip the 'write' part. Hit `:q` then **Enter**. You might be prompted with '**E37: No write since last change \(add ! to override\)**'. So let's follow the instructions there. Hit `:q!` then **Enter**. Use `cat` again to confirm your changes weren't saved.

12. Let's now work with `cp` and `rm`** **to make copies of our file and remove files. Run `cp CLIFun CLIFun2`. If you do an `ls -al` you'll see there's now a **CLIFun2** file with the same size as the **CLIFun** file but a more current timestamp. Ok, let's undo that by running `rm CLIFun2`.

13. Let's try copying a directory as well. Run `cp CommandLineBasics CommandLineBasics2` after changing into the CodingandCocktails parent directory. Oh no, we got an error again: '**cp: CommandLineBasics is a directory \(not copied\)**'! It looks like `cp` doesn't work with directories, but actually, we can copy a directory by adding an option to `cp`. We'll add a **-r** for **recursive**. So let's run `cp -r CommandLineBasics CommandLineBasics2`. Don't forget your tab completion! This time, you'll see a **CommandLineBasics2** directory that's the same as the directory we copied it from, except that it has a more current timestamp. To remove the directory, use the recursive option again by running `rm -r CommandLineBasics2`.

14. What if we need to move a file? Well, then use **mv**! The proper syntax for the command is `mv <source> <destination>`. For the file we created earlier, you can use `mv ~/CodingandCocktails/CommandLineBasics/CLIFun ~/CodingandCocktails/`. If you're in the CodingandCocktails directory, using the command `mv CommandLineBasics/CLIFun .` will also work. Remember, '**.**' is a shortcut for the current directory.

15. Another command that's useful for files is `wc`. You can remember it as **word count**, and it'll be in the syntax `wc [options] filename`. Here are some available options you can try out:![](/wc_options.png)

16. Give it a shot on your own now! If you need a visual aid, follow the animation below.



