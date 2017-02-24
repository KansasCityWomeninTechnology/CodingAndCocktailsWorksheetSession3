# Part 4: Pipes & Redirects

---

#### Passing Output to a Program or File

**Pipe** is used to pass output to another **program or utility**. **Redirect** is used to pass output to either a **file or stream**. Let's start by looking at an example of redirecting to a stream.

A stream is input/output of data travelling between processes which can be standard input \(stdin\), standard output \(stdout\), and standard error \(stderr\).

1. Type `sort << END` and enter in all of the cocktail names you can recall.
2. The **END **can actually be any word you want. You're telling **sort** to accept input until a specific value is given.

You can also redirect to a file. Let's a make a list of our favorite beverages. We'll use the $MY\_FAV variable from before.

1. Enter `echo "My favorite cocktail is a" $MYFAV > fav_cocktail.txt`, then `cat fav_cocktail.txt` to see the results.
2. Let's add our second favorite cocktail. Type `echo "My favorite cocktail is a Moscow Mule" > fav_cocktail.txt`, then `cat fav_cocktail.txt`.

Hmm, what happened there? Oh, we'll actually need to use the redirect to **append** instead! Let's try that again.

1. Enter `echo "My favorite cocktail is a" $MYFAV > fav_cocktail.txt`, then `cat fav_cocktail.txt`.
2. To add your second favorite cocktail, type `echo "My favorite cocktail is a Moscow Mule" >> fav_cocktail.txt` then `cat fav_cocktail.txt`.

The commands `more` and `less` are also useful. You'll need to pipe them to the `cat` command. A pipe is a chain of processes so that output of one process \(stdout\) is fed to the input \(stdin\) to another. We'll use the `history` command in the examples below. This command is very useful if you're needing to search through your previous commands.

1. In your command line, type`history > history.log`.
2. Now enter `cat history.log | less`.
3. * You'll see '**:**' at the bottom of the terminal. Hit Enter to continue scrolling or hit 'q' to quit.

You can also chain redirects and pipes. Here are a couple of examples to try:

1. Enter `sort -r < history.log > history_sorted.txt`, then type `cat history_sorted.txt | less` to scroll through your sorted list.

   * The `sort` command is just what it sounds like. The `-r` is there so we can reverse the order of the sort.

2. Type `history | sort -r > history_pipesorted.txt`, then type `cat history_pipesorted.txt | less` again.

3. Enter `history | grep cat | sort -r > history_grep.txt`, then `cat history_grep.txt`.



