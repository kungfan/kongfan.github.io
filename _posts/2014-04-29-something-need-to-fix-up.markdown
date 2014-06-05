---
layout: post
location: Huang Gang
---

Q : how to quote code section such as `{% raw %}{% include disqus_comment %}{% endraw %}` ?   
A : you can use `{% raw %}{% raw %} ...{ % endraw %}{% endraw %}` to lose sight of liquid tags

Q : when a file edited by vim no windows , there would be many `^M` How to deleted `^M`?    
A : we strip thoese characters by `%s/\r//g` or `%s/ctrl-v M//g` see also [here](http://vim.wikia.com/wiki/File_format)

Q : how to make Sublime Text support chinese ?
A : you can install [Control.sublime-package](http://sublime.wbond.net/Package%20Control.sublime-package),then restart Sublime Text.

Q : how to set vim  automatic word wrapping ?
A : You can set the text width using `:set textwidth=n` (or :set tw=n) such as` :set tw=79`

Q : How to delete *Byte-Order mark*`(BOM)` ?
A : Notepad++ provides a useful function that can save UTF-8 files without BOM header. So,  just use it to deal with the BOM header problem.
