A Fork of Fletcher Penney's Markdown TextMate bundle, incorporating some new commands:

`hyper ⇥` will insert a hyperlink in the following format: `[Link text](URL "Title")`  
You can switch between the link text, url, and title fields by pressing tab.  

`cite ⇥` will insert a BibTex/BibLaTeX citation field in the following format: `[abb. page number/chapter/scene][#Author:year+identifier]`  
You can switch between the abb., number, author, and year+identifier fields by pressing tab.  

`⌘ + ⌥ + f` will create a footnote at the caret position. **This is currently experimental**. It assumes that all your footnotes are in the format `[^n]`, where `n` is a positive integer greater than 0. Place the caret at the position you want the footnote to appear, then use the key combination. A new footnote anchor will be created, and at the bottom of your document, a blank line will be inserted, followed by the matching footnote and a text field. Pressing  ⇥ (tab) once should jump from the caret to the footnote text, and pressing tab again should jump back up to the caret position. The macro inserts a blank line above each successive footnote, as LaTeX (or perhaps MMD) won't process them properly otherwise. Feel free to remove the leading newline from the macro if you never convert to LaTeX. Many thanks to ‘Dr Drang’ (I have no idea. It's the Internet, what do you want from me?) from the TextMate list for some Perl pointers. I am so bad at writing Perl that I probably have no business being on Github. Also, my facial hair is quite neat. Speak of this to no-one. 


