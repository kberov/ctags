Extended Rules to support Modern Perl in Exuberant Ctags
=====
This is my Exuberant Ctags (~/.ctags) file.
I use it with jEdit + CtagsInterface and Ctags Sidecick plugins. 
It can be used with many other editors
like Vim, Emacs, jEdit, Sublime Text...

For now it only contains some additional regular expressions 
to support more Perl symbols.
Feel free to contribute by adding regular expressions!

Usage
===
Just put the file in your $HOME folder.


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

Красимир Беров (2013)
