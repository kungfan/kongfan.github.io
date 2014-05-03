---
layout: post
---

Q : how to quote code section such as ` { % include disqus_comment % } ` ?   
A :

Q : when a file edited by vim no windows , there would be many `^M` How to deleted `^M`?    
A : we strip thoese characters by `%s/\r//g` or `%s/ctrl-v M//g` see also [here](http://vim.wikia.com/wiki/File_format)
