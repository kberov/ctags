Extended Rules to support Modern Perl in Exuberant Ctags
=====
This is my Exuberant Ctags (~/.ctags) file.
I use it with Vim and Atom. 
It can be used with many Text editors
like Vim, Emacs, jEdit, Sublime Text, Atom...

For now it only contains some additional regular expressions 
to support more Perl symbols. Feel free to contribute by adding
regular expressions or improving the existing ones! Pull requests are wellcome.

Usage
===
Just put the file in your $HOME folder.

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

Bugs and limitations
===

Currently it does not handle POD after the __END__ marker.

Author
===

Красимир Беров (2013--2017)
