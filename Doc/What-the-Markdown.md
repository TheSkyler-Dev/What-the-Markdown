# What the Markdown - An example of a good Documentation that teaches you Markdown!
## Table of Contents
1. [Getting Started](#getting-started)
2. [Basic text styles](#basic-text-styles)
3. [Lists](#lists)
4. [More text styles](#more-text-styles)
5. [Quoting text](#quoting-text)
6. [Inserting code and code blocks](#inserting-code-and-code-blocks)
7. [Making a table of contents](#making-a-table-of-contents)
8. [Embedding links](#embedding-links)
9. [Embedding images](#embedding-images)
10. [Embedding badges](#embedding-badges)
11. [Closing thoughts](#closing-thoughts)
---
## Getting Started
Markdown is a simple and lightweight markup language that lets you format text so it's more structured and readable. It plays a big loe in our everyday lives - without us noticing. It also plays a huge part in the life of a **software engineer**! GitHub, GitLab, Obsidian, Jupyther notebooks and even Discord messages use or support Markdown to some capacity in their own ways. The most common form of Markdown is **standard Markdown**, which is fully supported by GitHub, GitLab and Obsidian, just to name a few. In this document, you will learn the *basics* of the **standard implementation of Markdown**.
## Basic text styles
In Markdown, there are quite a few different formats or *styles* your text can take on. Here are the **essential** formats that you likely will use the most, as those are **essential** to structuring your Documentation:

Headings:
```md
# Heading 1
## Heading 2
### Heading 3
```
The result:

![headings](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/Headings.png)

Bold text:
```md
**bold text**
```
The result:

![Bold text](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/Bold.png)

Italics:
```md
*italicized text*
```
The result:

![Italics](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/Italics.png)

## Lists
Lists are essential to organise bulletpointts, make rankings or make a table of content. In Markdown, there are two types of lists: Ordered and unordered lists. Here are some examples:

Unordered lists start with a dash followed by space and the bulletpoint text. Most markdown text editors will automatically add a new bulletpoint in a new line when you press enter:
```md
- item 1
- item 2
- item3
```
Result:

![Unordered List](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/UnorderedList.png)

Ordered lists start with a number and a full stop, followed by a space and text. Most text editors will automatically set the next number for you:
```md
1. item 1
2. item 2
3. item 3
```
Result:

![Ordered List](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/OrderedList.png)

## More text styles
Of course, there are more than the previously mentioned text formatting options, such as strikethrough and highlighting, though highlightin isn't supported by all Markdown editors. For example, GitHub doesn't support text highlighting.

To highlight text in markdown editors that support it, just wrap the text to be highlighted in double equal signs (`==`):
```md
==This is important==
```
Result:

![Highlighted text](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/Highlight.png)

To strikethrough text, simply place two tildes (`~`) in front and after the text that is to be struck through:
```md
~~The world is flat~~
```
Result:

![strikethrough](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/Strikethrough.png)

## Quoting text
Quoting text can be useful to quote someone or something, emphasize information and commentary, styling messages in documentation and more. To make a block quote, just start a line with a greater than (`>`) sign:

```md
> This is an example block quote
> It is very useful
```

Result:

![Block quote](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/Blockquote.png)

## Inserting code and code blocks
Inserting code or fenced code blocks in Markdown is useful to give code examples and explaining syntax in a documentation.
a single line code snippet can be made by wrapping text in single bacticks (`). For example:
```md
`<args>`
```
becomes `<args>`.

Fenced code blocks allow you to insert larger code snippets into your document. To do that, just place three backticks above and below the code snippet. You can also specify the programming language of the fenced code block by specifying it immediately after the top three backticks, which, on GitHub and GitLab will apply the appropriate syntax highlighting to the code block. Here's an example with a Hello World program written in Ada:
```md
```Ada
with Ada.Text_IO;

procedure Greet is
begin
   -- Print "Hello, WorlD!"
   Ada.Text_IO.Put_Line ("Hello, World!");
   Ada.Text_IO.Put_line ("Hello, Ada!");
end Greet;
``` )
```
> Please note that the closing parentesis does not have to be there. It was added to make that fenced code block work roperly.
> If you put a fenced code block within a fenced code block, it will take the first triple backticks without a type identifier as its closing triple backticks.

Becomes:

```Ada
with Ada.Text_IO;

procedure Greet is
begin
   -- Print "Hello, WorlD!"
   Ada.Text_IO.Put_Line ("Hello, World!");
   Ada.Text_IO.Put_line ("Hello, Ada!");
end Greet;
```

## Making a table of contents
A table of contents is an essetial part of a proper documentation. It lets readers easily navigate between chapters (marked by headings) with a single click. A table of contents always uses an ordered list of link embeds that refer to each chapter by their heading IDs:
```md
1. [Getting Started](#getting-started)
2. [Basic text styles](#basic-text-styles)
3. [Lists](#lists)
4. [More text styles](#more-text-styles)
5. [Quoting text](#quoting-text)
6. [Inserting code and code blocks](#inserting-code-and-code-blocks)
7. [Making a table of contents](#making-a-table-of-contents)
8. [Embedding links](#embedding-links)
9. [Embedding images](#embedding-images)
10. [Embedding badges](#embedding-badges)
11. [Closing thoughts](#closing-thoughts)
```
Becomes:

![Table of contents](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/TableOfContents.png)

## Embedding links
Embedding Links lets you refer to external sources and, as well as make a Table of contents (as shown in the previous section).
A link embed consists of the link text (enclosed in square brackets) and the link itself (enclosed in parentheses):
```md
[Google](https://google.com)
```
Becomes: 

![Link Embed](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/LinkEmbed.png)

## Embedding images
Embedding images is as easy as embedding links and generally uses the same syntax, but prefixed with an exclamation mark:
```md
![example](C:\Path\To\example.jpg)
```
Result:

![example](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/Img/ExampleImageEmbed.png)

## Embedding badges
Badges are a very popular feature in Documentations and README files on GitHub and GitLab and can show additional information, such as which version is current or which builds are passing or failing. These badges, often generated with [Shields.io](https://shields.io/badges), are embedded the same way images are embedded:
```md
![Static Badge](https://img.shields.io/badge/Example-Badge-blue?style=flat)
```
Result: ![Static Badge](https://img.shields.io/badge/Example-Badge-blue?style=flat)

## Closing thoughts
In this documentation you learned the basics of Markdown. Now you are well prepared to write your own, well structured documentations and at the same time, had a look at what a proper Documentation could look like! There is, of course, also some more advanced syntax in Markdown that we didn't discuss here, but if you want to check it out anyway, you can do so [here](https://www.markdownguide.org/cheat-sheet/). Feel free to switch this Documentation to the [code preview](https://github.com/TheSkyler-Dev/What-the-Markdown/blob/main/Doc/What-the-Markdown.md?plain=1) to see how it's built under the hood! You can do the same with another example documentation [here](https://github.com/TheSkyler-Dev/What-the-Markdown/tree/main/More-Doc-Examples).
