# Redirection & Pipes {#top}


{% hint style='tip' %}
While following along with the worksheet, type out the commands instead of doing a copy & paste unless explicitly stated to avoid inadvertently using any wrong characters.
{% endhint %}

<!-- trick markdown to give me a little space between these two sections of text -->
## 

This section will help guide you through the following steps:

{% include "./instruction-steps.html" %}

## Redirecting output {#redirects} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Use redirects to pass output to a **file or stream**. A stream is input/output of data travelling between processes which can be standard input \(stdin\), standard output \(stdout\), and standard error \(stderr\). Let's start by looking at an example of redirecting to a file.
{% include "./1redirects.md" %}

## Edit files {#edit} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Sometimes we need to edit files. We can do this in the CLI using a powerful text editor called vim.
{% include "./2vim.md" %}

## Searching {#search} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
The CLI has a built in capability to search. Let's try searching files.
{% include "./3search.md" %}

## Piping commands {#pipes} <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
Use a pipe to pass output to another **program or utility**. A pipe can chain processes so that output of one process \(stdout\) feeds into the input \(stdin\) of another.
{% include "./4pipes.md" %}

<!-- trick markdown to give me a little space between these two sections of text -->
## 

## References and helpful links <span class="navigate-top"><a href="#top" title="Take me to the top of page"><i class="fa fa-chevron-circle-up" aria-hidden="true"></i></a></span>
[GNU/Linux Command-Line Summary for directing input/output](https://linux.die.net/Linux-CLI/usage-input-output.html)

[GNU/Linux Command-Line Summary for text related tools](https://linux.die.net/Linux-CLI/text-related-tools.html)

[GNU/Linux Command-Line Summary for searching](https://linux.die.net/Linux-CLI/finding-text-within-files.html)



