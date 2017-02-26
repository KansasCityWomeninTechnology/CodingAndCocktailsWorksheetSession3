# Part 2: Manipulating Files

---

#### Create and Edit Files and Directories

Let's get straight to learning how to manipulate files and directory structures!

1. Change into your home folder by typing `cd ~`. Type `ls -al` to check if a **CodingandCocktails** folder already exists.
   * If it doesn't, create it using `mkdir CodingandCocktails`. Note that the command line is **CASE-SENSITIVE**, so watch your capitalization!
2. In your CodingandCocktails folder, create a **CommandLineBasics** folder by entering in `mkdir CommandLineBasics`.

3. Let's create a file by typing `touch CLIFun`.

Now, we'll want to add some content to your file.

1. Open your file in vim by typing `vim CLIFun`.

   * While **vim** is one option for a text editor, there are many others available. You can use this [**vim cheat sheet**](https://vim.rtorr.com/)** **to take full advantage of** **its powerful features.

What's with all the squigglies?!? Don't worry! By learning a few basic vim commands, you'll be saving contents in your files in no time. Let's start by copying the [**lorem ipsum**](https://en.wikipedia.org/wiki/Lorem_ipsum) text below.

1. ```
   Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
   et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut 
   aliquip ex ea commodo consequat.
   ```
2. Go back to iTerm2/Git Bash and hit `i`. That'll put you into **INSERT** mode.

3. Now hit **⌘V** on your Mac or **CTRL + V** on your Windows laptop to paste the text you copied.

4. Next, type in `:wq` and then hit **Enter**. Awesome, now we've got some content to play with!

   * The 'w' stands for **write** and the 'q' stands for **quit**.

5. Now type `cat CLIFun` to display the contents of the file. Cool!

6. To add more content, type `vim CLIFun` to enter the editor again. Hit `i` again like we did before and start entering in some text.

But that messed up our lorem ipsum sample! What to do?!? No worries, let's just close out of the text editor without saving our changes. We did a 'write' and then 'quit' earlier, let's instead skip the 'write' part.

1. Hit `:q` then **Enter**. 
   * You'll be prompted with '**E37: No write since last change \(add ! to override\)**'. If so, follow the instructions there. Hit `:q!` then **Enter**. 
2. Type `cat CLIFun` again to confirm your changes weren't saved.

Let's now work with `cp` and `rm`** **to make copies of our file and remove files.

1. Type `cp CLIFun CLIFun2`.

   * If you do an `ls -al` you'll see there's now a **CLIFun2** file with the same size as the **CLIFun** file but a more current timestamp.

2. Ok, let's undo that by entering `rm CLIFun2`.

Let's try copying a directory as well.

1. Type `cp CommandLineBasics CommandLineBasics2` after changing into the CodingandCocktails parent directory.

   * Oh no, we got an error again: '**cp: CommandLineBasics is a directory \(not copied\)**'! It looks like `cp` doesn't work with directories, but actually, we can copy a directory by adding an option to `cp`. We'll add a **-r** for **recursive**. 

2. Let's try that again. Type `cp -r CommandLineBasics CommandLineBasics2`.

   * Don't forget your tab completion! This time, you'll see a **CommandLineBasics2** directory that's the same as the directory we copied it from, except that it has a more current timestamp. 

3. To remove the directory, use the recursive option again by typing `rm -r CommandLineBasics2`.

   * Be **VERY** careful when running rm commands. If you do it from  the wrong directory, you could potentially remove your entire **OS** \(**O**perating **S**ystem, i.e. Windows or Mac OSx\) or other really important data!!

What if we need to move a file? Well, then use **mv**! The proper syntax for the command is `mv <source> <destination>`.

1. Type `mv ~/CodingandCocktails/CommandLineBasics/CLIFun ~/CodingandCocktails/`.

   * If you're in the CodingandCocktails directory, the command `mv CommandLineBasics/CLIFun .` will also work. Remember, '**.**' is a shortcut for the current directory.

Another command that's useful for files is `wc`. You can remember it as **word count**, and it'll be in the syntax `wc [options] filename`. Here are some available options you can try out:

![](/wc_options.png)

Give it a shot on your own now! If you need a visual aid, follow the animation below.

![](/assets/CLI01.gif)

