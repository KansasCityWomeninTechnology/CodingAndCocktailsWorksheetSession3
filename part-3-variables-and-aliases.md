# Part 3: Variables & Aliases

---

#### Using Variables and Making Aliases

Alternatively, you could use sed:

history \| sed 's/^\[ \]\*\[0-9\]+\[ \]\*//'

Using alias, you can set this as your standard \(stick it in your bash\_profile\):

alias history="history \| sed 's/^\[ \]\*\[0-9\]+\[ \]\*//'"

built in \(date\), create one, PATH, alias, how to make permanent, $MY\_FAV

