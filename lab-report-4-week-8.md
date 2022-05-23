# Lab report 4
## Required links
- [My Markdown-parser repository](https://github.com/astoriama/markdownParse-for-report4.git)
- [Reviewed Markdown-parser repository](https://github.com/ima-quack/markdown-parser.git)


## Snippet 1
### Expected Product:
![snippet1expected](snippet1expected.png)
### Code in `MarkdownParseTest.java`:
![code1](code1.png)
## Testing and fixing my implementation:
![myResult1](myResult1.png)
My code failed due to the reason that I never considered such quotation marks' priority as in the first link. I believe I could fix the code by adding an if statement at the begining, to determine whether their exists such quotation marks. If such quotation exists, than prioritize such quotation mark.
## Testing other's implementation:
![othersResult1](othersResult1.png)


## Snippet 2
### Expected Product:
![snippet2expected](snippet2expected.png)
### Code in `MarkdownParseTest.java`:
![code2](code2.png)
## Testing and fixing my implementation:
![myResult2](myResult2.png)
This failure is because I failed to consider the possibility of having two closing paranthesises in the link. However, I do not think I can fix such issue in short lines. I had tried multiply times in previous labs, and failed.
## Testing other's implementation:
![othersResult2](othersResult2.png)


## Snippet 3
### Expected Product:
![snippet3expected](snippet3expected.png)
### Code in `MarkdownParseTest.java`:
![code3](code3.png)
## Testing and fixing my implementation:
![myResult3](myResult3.png)
This failure is due to lack of consideration of blankspace. In order to fix such issue, we just need to let the `currentIndex` add one when it meet blanksapce, to skip blankspace and restore correct format.
## Testing other's implementation:
![othersResult3](othersResult3.png)
