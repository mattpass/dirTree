dirTree
=======

PHP file &amp; folder dir tree generator

Creates a file & folder list (dir tree) using PHP's own inbuilt iteration functions to create a dir tree.

This has big advantages over the usual recursion methods (using scandir for instance) which are inefficient and therefore slow.

Here are perf tests 5 times in a row, using the 2 methods:

```**Usual recursive method (scandir etc)**
6.51, 6.27, 6.92, 6.56 and 6.73 secs
= 32.99 secs = **6.59 secs avg**```

```**The above method iteration method**
3.38, 3.26, 3.24, 3.40 and 3.23 secs
= 16.51 secs = **3.30 secs avg**```

(Tested 5 times in a row on a server with 2,120 files in 248 folders with a size of ~110mb)

The output is a HTML UL based list which no formatting etc so you have a clean start point to reformat, create links etc

**Demo:**
http://icecoder.net/dir-tree.php
(View the source to see clean & tidy code)

Feel free to use for any purpose (MIT licensed) & put forward issues & pull reqs if you can improve.

Happy usage! :)