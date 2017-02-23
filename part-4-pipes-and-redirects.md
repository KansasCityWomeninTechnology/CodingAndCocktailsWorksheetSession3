# Part 4: Pipes & Redirects

---

#### Passing Output to a Program or File

**Pipe** is used to pass output to another **program or utility**. **Redirect** is used to pass output to either a **file or stream**. Let's start by looking at an example of redirecting to a stream.

1. Type `sort << END` and enter in all of the cocktail names you can recall.
   * The **END **can actually be any word you want. You're telling **sort** to accept input until a specific value is given.

You can also redirect to a file. Let's a make a list of our favorite things.

1. Enter `echo "My favorite cocktail is a" $MYFAV > fav_cocktail.txt`, then `cat fav_cocktail.txt` to see the results.
2. Let's add our second favorite cocktail. Type `echo "My favorite cocktail is a Moscow Mule" > fav_cocktail.txt`, then `cat fav_cocktail.txt`.

Hmm, what happened there? Oh, we'll actually need to use the redirect to append instead! Let's try that again.

1. Enter `echo "My favorite cocktail is a" $MYFAV > fav_cocktail.txt`, then `cat fav_cocktail.txt` to see the results.
2. To add your second favorite cocktail, type `echo "My favorite cocktail is a Moscow Mule" >> fav_cocktail.txt`, then `cat fav_cocktail.txt`.

The commands **more**, **less**, and **grep** are also useful. Remember the CLIFun file we created earlier in [**Part 2**](/content/part-2-manipulating-files.html)?

