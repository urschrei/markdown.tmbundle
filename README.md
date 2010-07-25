A Fork of Fletcher Penney's Markdown TextMate bundle, incorporating some new commands:

`hyper ⇥` will insert a hyperlink in the following format: `[Link text](URL "Title")`  
You can switch between the link text, url, and title fields by pressing tab.  

`cite ⇥` will insert a BibTex/BibLaTeX citation field in the following format: `[abb. page number/chapter/scene][#Author:year+identifier]`  
You can switch between the abb., number, author, and year+identifier fields by pressing tab.  

**TO DO:**  
Figure out a sensible footnote insertion snippet. This isn't going to be easy, because I'm going to have to remember enough Ruby to jump to the end of the document or section, and then back to the insertion point. Also, I can't think of any sensible way to automatically insert a footnote identifier: using line numbers won't work because you could have multiple footnotes on the same line, and line insertion during editing could ruin everything. Perhaps an MD5 hash of the current date and time would work. Hmm.
