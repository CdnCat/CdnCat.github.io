---
layout: post
title: "Bash exit codes"
---

<h4>[1 minute read]</h4>

In many languages, 0 is considered a falsy value. However in the shell, 0 indicates a successful process while a non-zero return value would indicate an unsuccessful process. This is important to remember when you're writing a shell script:

<pre>
ls | grep -q README && echo 'README exists'
</pre>

Read more <a href="https://stackoverflow.com/q/2933843/6342085">here</a>.
