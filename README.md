Extended Rules to support Modern Perl in Exuberant Ctags
=====
This is my Exuberant Ctags (~/.ctags) file.
I use it lately with Vim with the tagbar plugin. 
It can be used with many Text editors
like Vim, Emacs, jEdit, Sublime Text, Atom...

For now it only contains some additional regular expressions 
to support more Perl symbols. Feel free to contribute by adding
regular expressions or improving the existing ones! Pull requests are wellcome.

Usage
===
For generating tags file with ctags, just put the file in your $HOME folder.

To add the content of this file to your existing ~/.ctags file:
```bash
curl https://raw.githubusercontent.com/kberov/ctags/master/.ctags >> ~/.ctags
```
If you are using Atom, you don't need this file, because its content is already part
of the [symbols-view](https://atom.io/packages/symbols-view) core package.

How to add support for new symbols?
===

http://ctags.sourceforge.net/

http://stackoverflow.com/questions/979359/vim-and-custom-tagging

https://ericjmritz.wordpress.com/2013/03/14/writing-custom-rules-for-exuberant-ctags/

Make it work with tagbar vim plugin
====

Add the following to your .vimrc.
The [tagbar plugin](https://github.com/majutsushi/tagbar) has to be used ofcourse.

```vim
let g:tagbar_type_perl = {
    \ 'ctagstype' : 'perl',
    \ 'kinds'     : [
        \ 'p:package:0:0',
        \ 'w:roles:0:0',
        \ 'e:extends:0:0',
        \ 'u:uses:0:0',
        \ 'r:requires:0:0',
        \ 'o:ours:0:0',
        \ 'a:properties:0:0',
        \ 'b:aliases:0:0',
        \ 'h:helpers:0:0',
        \ 's:subroutines:0:0',
        \ 'd:POD:1:0'
    \ ]
\ }

```

Bugs and limitations
===

POD after the __END__ marker is not shown, but seems this is caused by ctags and I don't have an idea how to change it.

Author
===

Красимир Беров (2013--2018)
