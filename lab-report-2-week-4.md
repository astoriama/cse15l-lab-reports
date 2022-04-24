# Lab Report 2 Week 4
### 3 changes to MarkDownParse.java
---
## First Change: Allow paratheses in links
<img src="CorrectionLink1.png"
     alt="CorrectionLink2"
     style="float: left; margin-right: 10px;" /> 

Link to the test file for a failure-inducing input that prompted you to make this change is [here](https://github.com/astoriama/markdown-parser/commit/d0a6a357b7a569e9424167a06e03bda0c65eb455).

An unexpected output in shown as:
```
Exception in thread "main" java.lang.OutOfMemoryError: Java heap space
        at java.base/java.util.Arrays.copyOfRange(Arrays.java:3822)
        at java.base/java.lang.StringLatin1.newString(StringLatin1.java:769)
        at java.base/java.lang.String.substring(String.java:2709)
        at MarkdownParse.getLinks(MarkdownParse.java:19)
        at MarkdownParse.main(MarkdownParse.java:30)
```

The failure is caused by extra paratheses in the link in the file. The original code take in the first closing paratheses it sees and make mistake because it can not find the next correct symbol. However, I altered the code so that it use the last paratheses it sees, which will lead it to its' correct way.

