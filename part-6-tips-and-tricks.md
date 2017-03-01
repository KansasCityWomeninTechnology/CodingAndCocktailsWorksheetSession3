# Part 6: Tips & Tricks

---

#### Better, Faster, Stronger!

Below is a list of more useful stuff and shortcuts. Try them out!

**Commands**:

* `date` - will show you the current system date
* `hostname` - shows the machine name you're currently logged into
* `head` - prints out the first `-n` lines of a file \(defaults to 10\)
* `tail` - similar to head, prints out the last -n lines of a file \(also defaults to 10\)
  * `tail -nf` will continue to show the last _n_ lines of a file so that if it's updated, the output will be as well
* `clear`- will clear your terminal
* `whoami` - tells you the username that you're logged in as
* `uptime` - displays how long your machine has been up
* `ping` - checks to see if a reply is received from a remote location
  * Example: `ping towel.blinkenlights.nl`
* `history`- lists out the prior history of commands
* `!!` - allows you to repeat the last command ran; you can also append to it like this:
  * For example, if the last command you ran was `history`, you could then run `!! | grep cat` and you would get the same output of all of the listed items in history that included the string 'cat'.
* `sudo` - used when elevated permissions are required
  * `sudo !!` would append `sudo` to the beginning on the last command ran. This is especially useful when you forget to use elevated, or `sudo`, privileges with a command.

**Get help \(super useful!\)**:

* `man` - shows you the manual or help page of a command, often including syntactical examples
  * For example, `man chmod` will give you information on how to use the `chmod` command and what it does.
* `/?`, `--help`, or `-h` - will show help text of a command; to be used in the format `<command> /?`, for example

**Moving around at the CLI prompt**:

* **Ctrl + U**: Clears the line from the cursor point back to the beginning.

* **Ctrl + A**: Moves the cursor to the beginning of the line.

* **Ctrl + E**: Moves the cursor to the end of the line.

* **Ctrl + R**: Allows you to search through the previous commands

**Have some fun**:

Ever wondered what _Star Wars: Episode IV_ would look like in all text? Of course you have! Let's find out:

1. Type `telnet towel.blinkenlights.nl` and hit Enter.
    {% hint style='info' %}
   * `telnet` is a protocol that allows you to log in to another remote machine, located in this case at towel.blinkenlights.nl.
   {% endhint %}



