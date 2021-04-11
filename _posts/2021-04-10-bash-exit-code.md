---
layout: post
title: "Bash exit codes"
---

<h4>[1 minute read]</h4>

In many languages, 0 is considered a falsy value. However in the shell, 0 indicates a successful process while a non-zero return value would indicate an unsuccessful process. This is important to remember when you're writing a shell script:

<pre>
grep_exit_code=$(ls | grep -q README; echo $?)
echo $grep_exit_code # 0
if [ grep_exit_code ]
  then
    echo "hello world"
fi
</pre>

Read more about the above <a href="https://stackoverflow.com/q/2933843/6342085">here</a>.  
Read more about the `$?` <a href="https://stackoverflow.com/q/6834487/6342085">here</a>
