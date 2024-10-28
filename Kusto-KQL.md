# Table of Contents

<!-- vscode-markdown-toc -->
* 1. [String manipulation](#Summary)
* 2. [Regex](#Features)
* 3. [Usage](#Usage)
* 4. [Configuration](#Configuration)
* 5. [Example](#Example)
* 6. [About](#About)
* 7. [Roadmap](#Roadmap)

<!-- vscode-markdown-toc-config
    numbering=true
    autoSave=true
    /vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->


## 1. <a name='String manipulation'></a>String manipulation 

#### Split:
Example 1
```kusto
DeviceFileEvents
| extend FileExtension = split(FileName,".")[-1]
```
Spilt the string FileName at the "." and assign the value to FileExtension

Example 2
```kusto
DnsAudit_CL
| extend Account = split(split(values[0],"(")[-1],")")[0]
```
Assign Account with the string between the two paranthes ()
:bulb: **Tip:** [-1] means the last past

[link](Powershell.md "Powershell.md")
[link](Python.md)

# Heading

---

## Sub Heading

1. item 1
2. item 2
3. item 3


tedst

1. [link](Strings.md) "String manipulations"
2. [link](Regex.md) "Regular expressions"
3. [link](DatesTimes.md) "Working with date & times"

*this is italic*

**This is bold text**

# Links
[Link here](http://dr.dk "hover over text")

[Links](#links)
[cs]: https://youtube.com/

[CodeStackr][cs]

-[x] checklist
-[ ] test

sql `map()` code

Fenced code block :
```
select * from dual;
```
1. js - javascript
2. py - python

#blockquote
> this is a blockquote
>
> some more text
>  >reply

# Images

![alt text goes here](/codecat.png)

[![alt text goes here](/codecat.png)](https://codecats.xyz)

# Tables

| col1 | col2 | col3 |
| :--- | :---: | :--- | 
| test | car | girl |

# task list
- [x] Task 1
- [ ] Task 2
- [ ] Task 3


enjoy :-)

# Comments
[This is a hidden comment.]: #

#### Comment

# Toggle
<details>
    <summary>This is a toogle!</summary>
    Content of toggle.
</details>

# Callouts

> :bulb: **Tip:** Here is an important tip to remember!
> [link](https://www.youtube.com/watch?v=ftOBvusMHjQ)
> 
> [link](https://https://github.com/codeSTACKr/markdown-crash-course "kursus materiale")