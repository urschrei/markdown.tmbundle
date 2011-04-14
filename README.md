A Fork of Fletcher Penney's Markdown TextMate bundle, incorporating some new commands:

A variation on the 'Convert Document To PDF' command is available: **'Convert Document To PDF (XeLaTeX)'**. This uses a custom makefile to compile your MMD file into a PDF using [XeLaTeX](http://en.wikipedia.org/wiki/XeTeX "XeTeX"). This makefile can be obtained [here](https://gist.github.com/918097 "mmd3_proc.py"), and requires Python 2.7.x (it may work with 2.6.x, but is untested). The makefile should be put somewhere on your $PATH.

`hyper ⇥` will insert a hyperlink in the following format: `[Link text](URL "Title")`  
You can switch between the link text, url, and title fields by pressing tab.  

`cite ⇥` will insert a BibTex/BibLaTeX citation field in the following format: `[abb. page number/chapter/scene][#Author:year+identifier]`  
You can switch between the abb., number, author, and year+identifier fields by pressing tab.  

`⌘ + ⌥ + f` will create a footnote at the caret position. **This is currently experimental**. It assumes that all your footnotes are in the format `[^n]`, where `n` is a positive integer greater than 0. Place the caret at the position you want the footnote to appear, then use the key combination. A new footnote anchor will be created, and at the bottom of your document, a blank line will be inserted, followed by the matching footnote and a text field. Pressing  ⇥ (tab) once should jump from the caret to the footnote text, and pressing tab again should jump back up to the caret position. The macro inserts a blank line above each successive footnote, as LaTeX (or perhaps MMD) won't process them properly otherwise. Feel free to remove the leading newline from the macro if you never convert to LaTeX. Many thanks to [Dr. Drang](https://github.com/drdrang "Dr. Drang") from the TextMate list for some Perl pointers.  

