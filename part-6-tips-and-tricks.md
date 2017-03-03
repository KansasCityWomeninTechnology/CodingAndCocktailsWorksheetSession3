# Part 6: Tips & Tricks

---

#### Better, Faster, Stronger!

Below is a list of more useful stuff and shortcuts. Try them out!

**Commands**:

* `date` - will show you the current system date
* `hostname` - shows the machine name you're currently logged into
* `head` - prints out the first `-n` lines of a file \(defaults to 10\)
* `tail` - similar to head, prints out the last _n_ lines of a file \(also defaults to 10\)
    {% hint style='hint' %}
`tail -nf` will continue to show the last _n_ lines of a file so that if it's updated, the output will be as well.
    {% endhint %}
* `clear`- will clear your terminal
* `whoami` - tells you the username that you're logged in as
* `uptime` - displays how long your machine has been up
* `ping` - checks to see if a reply is received from a remote location
    {% hint style='hint' %}
Example: `ping towel.blinkenlights.nl`
    {% endhint %}
* `history`- lists out the prior history of commands
* `!!` - allows you to repeat the last command ran; you can also append to it like this:
    {% hint style='hint' %}
For example, if the last command you ran was `history`, you could then run `!! | grep cat` and you would get the same output of all of the listed items in history that included the string 'cat'.
    {% endhint %}
* `sudo` - used when elevated permissions are required
    {% hint style='hint' %}
`sudo !!` would append `sudo` to the beginning on the last command ran. This is especially useful when you forget to use elevated, or `sudo`, privileges with a command.
    {% endhint %}

**Get help \(super useful!\)**:

* `man` - shows you the manual or help page of a command, often including syntactical examples
    {% hint style='hint' %}
For example, `man chmod` will give you information on how to use the `chmod` command and what it does.
    {% endhint %}
* `/?`, `--help`, or `-h` - will show help text of a command when added as an option
    {% hint style='hint' %}
To be used in the format `<command> /?`. Example: `grep --help`.
    {% endhint %}
**Moving around at the CLI prompt**:

* Ctrl + U: Clears the line from the cursor point back to the beginning.

* Ctrl + A: Moves the cursor to the beginning of the line.

* Ctrl + E: Moves the cursor to the end of the line.

* Ctrl + R: Allows you to search through the previous commands

* Ctrl + C: Cancels out of current command

**Have some fun**!

Here's a couple of fun things you can do in the command line:

1. Ever wondered what _Star Wars: Episode IV_ would look like in all text? Of course you have! Type `telnet towel.blinkenlights.nl` and hit Enter.
    {% hint style='info' %}
The `telnet` command uses a **protocol** that allows you to log in to another remote machine, located in this case at towel.blinkenlights.nl. A protocol is a set of procedures and rules for data transmission.
    {% endhint %}

2. You can also play a fun game to sharpen your vim skills. Visit https://vim-adventures.com/.
