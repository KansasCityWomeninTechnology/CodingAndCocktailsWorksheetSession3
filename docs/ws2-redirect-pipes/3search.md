1. Now that we have files with content, let's try searching. We can search by using `grep`. Type `grep "Lorem" CLIFun.txt` <i class="fa fa-share fa-rotate-180"></i>. We see the line that matches the string "Lorem" in the terminal.

1. Let's search across all files in the "CommandLineBasics" directory. Type `grep "cocktail" *` <i class="fa fa-share fa-rotate-180"></i>. Now we see name of the file and the line that matches the string "cocktail".
JAD TODO Add picture here

1. We can get a count of matches too. Type `grep -c "cocktail" *` <i class="fa fa-share fa-rotate-180"></i>. Now we see the name of the file and number of matches in the file.
JAD TODO Add picture here
