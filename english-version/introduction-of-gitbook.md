Chapter 1: The Introduction of Gitbook
===
---

GitBook is a kind of command line tool(node.js repositories),using Github/Git to create exquisite books.Here is an example: [高效使用 Mac OS X](https://www.GitBook.com/book/prettyxw/mac-os-x-tricks/details). You can also publish books through the [GitBook.io](https://www.gitbook.com).The complete document is on the website [help.gitbook.com](help.gitbook.com).

#### Outputs
Gitbook's outputs has two types:

- **Static site**：Default site.Can be published in the Github Pages.
- **eBook**：After finishing the book,you can create your own eBook,the outputs can be  **PDF**, **ePub** or **MOBI**。

#### The Structure of the book

One book is one Git repository,and has two basic default documents: `README.md` and  `SUMMARY.md`.

	README.md is the introduction of your book，it would be added in the summary.

	SUMMARY.md defines the catalog of the book.It includes chapters lists and their links.

For example: Summary.md
<!-- lang:CSS -->
	# Summary
	This is the summary of my book.
	* [section 1](section1/README.md)
    	* [example 1](section1/example1.md)
	    * [example 2](section1/example2.md)
	* [section 2](section2/README.md)
    	* [example 1](section2/example1.md)
    
    Attention：First level title and  the second using unordered list such as“ +-*/ ”signals，and remember that you'd better using the same signal in one passage.
    You'd better distinguish the first level title and the second using two spaces and four spaces.The special symbols of the unordered list are separated from the text by spaces.
   
Files that are not included in `SUMMARY.md` will not be handled by` GitBook`.


