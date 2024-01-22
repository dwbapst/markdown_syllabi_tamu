# Syllabi Templates for Texas A&M Courses in Markdown Format

This is an unofficial, unapproved repositiory of syllabus templates in Markdown format that *should* meet the minimum syllabus requirements made by the Texas A&M Faculty Senate. This template was originally designed to meet the guidelines released in Fall 2020, and has been updated as recently as January 2024. The [original syllabus templace](https://facultysenate.tamu.edu/important-faculty-updates/minumum-syllabus-requirements) from the Faculty Senate was developed for use with Microsoft Word, which the author of this template finds noxious to use. 

The conversion to Markdown was done by David Bapst in the College of Geosciences, when it was the College of Geosciences, and updated later, when his academic unit was in the College of Arts & Sciences. Nothing about this repository's use of Markdown over Microsoft Word is approved by any entity at Texas A&M, and absolutely no inferences should be drawn from the fact that the author of this repository is currently serving on the faculty senate. Use this template at your own risk!

Markdown is a commonly used 'mark-up' language, indicating how text should be formatted and displayed but with minimal use of special characters or enclosures in the language. This minimalist 'lightweight' approach is (partly?) why it is called 'markdown', to differentiate it form more complex mark-up langugaes, like HTML and LaTeX. Many who use Markdown as their mark-up language of choice appreciate that it can be written in any plain-text editor, and the results of formatting can often be predicted easily -- this property is 'readability' and why it is often called a 'humane' mark-up language. (In a sense, markdown is humane because it is a markup language for humans.) Files that use the Markdown format often use a `.md` file extension. In fact, the readme you are reading was written and formatted with Markdown, and is natively displayed on Github as a formatted document. Other popular websites that use Markdown formatting are Discord and Reddit. Many have become well acquainted with Markdown in its use as a hybrid coding/formatting language for writing 'Rmarkdown' notebooks in RStudio, the popular interactive developer environment for the open-source statistical programming language, R. The author of this repository (me) chose Markdown for these syllabi templates as that formatting language can be quickly and efficiently converted to HTML or PDF via many tools, particularly Pandoc. 

# What are the Syllabus Requirements for Texas A&M Courses as Given by the Faculty Senate?

If we look at the guidelines documents and the associated template, the accessibility requirements for syllabi essentially are the following: the syllabus document should include a single level-1 heading (i.e., “Syllabus”) with three level-2 headings (i.e., “Course Information,” “University Policies,” and “College and Department Policies”). (Note from January 2024: At some point, a fourth level-2 header was added, "Campus Policies", listed on the syllabus template shown in Canvas, and which contains a section of text about FERPA.) 

The “Course Information” and “University Policies” sections (and, more recently, the "Campus Policies" section) have their own subsections identified with level-3 headers. Occassionaly, a level-3 header will have its own subsections with level-4 headers but this is uncommon. 

To use this syllabus template, just as they do with the provided Word document templace or the associated web template on Canvas, faculty should edit the content in the “Course Information” sections to include the appropriate details for the specific course they are teaching, and review the text included in the “University Policies” section. 
The TAMU Faculty Senate established the wording of the text in the University Policies section. Faculty associated with the main campus in College Station should use the Academic Integrity, Americans with Disabilities Act, and Title IX statements as written. (Note that there were slight cosmetic changes to the wording of these sections between 2020 and 2024.) 
Faculty not on the main campus should use the appropriate language and location at their campus for the Academic Integrity, Americans with Disabilities Act, and Title IX statements, and not edit any of these written statements. As described in the syllabus template, faculty member may add separate paragraphs if additional information is needed. Faculty should also add subsections for college level and/or department level policies as appropriate for their respective units. 
Faculty should use Heading level-3 for any new headings added under the College and Department Policies section. In Markdown, a level-3 header can be denoted by a line beginning with three hash symbols, eg: `### My Level-3 Header`

More recently, an optional (maybe?) mental health statement was added to the template. However, while the services his statement refers to have changed name and administrative location, the statement found in the Canvas template has not changed, but (as of January 2024) the template in the Word document *has* changed.

# Converting Markdown Syllabi to Formatted Files with Pandoc

The template can then be converted to HTML using Pandoc -- open-source software which can be obtained for most operating systems (from this website)[https://pandoc.org/]. Go there, to their website, for more installation instructions and files. I apologize that those of you reading this with campus-owned machines may have difficulty getting the IT administrators who control your machines to install Pandoc. There are many converters you can find probably online, but to be honest, I don't trust websites like that so I am not going to recommend any. If you can, use Pandoc.

To use this syllabus template for creating a PDF, you must also have a LaTeX engine installed (and in your system's $PATH, if you are on a Windows machine). If you are on a Linux machine, you likely already have such, or can easily obtain such from a friendly local software package repository. This is somewhat more difficult on macOS or Windows, although if you have RStudio installed and often convert Rmarkdown files to PDF, you *probably* already have the requisite software installed, such as a TinyTEX distribution. 


To convert this file to a standard LaTeX-style PDF, all you need to do in the shell is (assuming your working directory contains the file in question):

```
# example of converting to PDF
pandoc syllabus_markdown.md -o test_syllabus.pdf 

# example converting to HTML
pandoc syllabus_markdown.md -o test_syllabus.html
```

Both of these commands will make a PDF and an HTML version of your syllabus that meet Faculty Senate requirements. You can also output many other types of files, including Word files.

# Formatting in Markdown

> "Its Dangerous To Go Alone, Take This!"

Formatting in Markdown is the essence of using 'tags' -- characters or specific sequences of characters -- to indicate different types of formatting for different types of text. Most importantly for this syllabus template, different levels of headers can be indicated by starting a line with a certain number of hash symbols (`#`) followed by a space and then text on that line as the header's title. 

Emphasis can be added to words or phrases in text, by inserting astericks (`*`) to either side of a word, sentence or phrase, such that the text between the astericks will be *italicized* (with just one set of astericks) or **bolded** (two sets of astericks, ex `**bolded**`). In some versions of Markdown, underscores, the `__` symbols, can also be used to add emphasis, but this isn't true in all versions of Markdown. Some instances of Markdown also have ways to designated strikethrough text (like ~~this text~~, the raw form of which is `~~this text~~` using double tildes) and also spoilered text (text that doesn't appear in an HTML document until it is clicked on, which will look something like ||this text||, the raw form of which is `||this text||` using double vertical bars). Neither of those might appear correctly in this read-me if you are reading it on Github because, as I said, their implementation is inexact and spotty.

URL links can be specified using the following format, where the text used to outwardly label the link is given in square brackets, and the URL is given in a follow set of parentheses. For example, `[this is a link to google](google.com)` becomes [this is a link to google](google.com). 

Note that successive lines will be considered as being successive sentences in the same paragraph, and thus some formatting like headers will not behave properly without blank lines before and after in the original markdown document. Bulleted lists can be generated easily by beginning successive lines (still seperated by a single blank line) with horizontal dashes (`-`) or single isolated asterisks (`*`).

We can also designate block quotes by beginning lines with a right-ward pointing carat (`>`), which may also be the symbol you think as a left-ward looking hungry alligator. Block-quotted text will then be usually depicted (when formatted) as indented blocks of text with a gray bar on the left, or a slightly different font. The line above below the header is an example of a block quote.

## Backticks for 'What You See Is What You Get' and Code Blocks

It may often be necessary to show text exactly as it is, without interpretation of tags, such as when trying to show code or (less commonly) when one is writing markdown documents that explain how to use markdown, like this document you are reading. This concept is sometimes referred to as What You See Is What You Get formatting, or WYSIWYG. To achieve such a mode in markdown, use the backtick (\`), a character you have likely never even realized was on your keyboard before, which usually can be made by holding down shift and hitting the tilde (`~`) key before the 1 on your keyboard. We can even create 'code blocks' for when we want to show longer snippets of computer code or other text, which will then usually be displayed in a monospace font. Code blocks can be initiated by a like with three 

```
hello!
This is a code block. 
It is made possible by the awesome and powerful ` backtick character
```

Code blocks like these probably don't have much use in writing syllabi with markdown, however. (Or maybe I just lack creativity! Prove me wrong!)

## Commenting in a Markdown Document

You may often want to leave behind comments that are useful to those editting future versions of a document (such as future versions of yourself) but would be distracting or confusing to anyone who is just reading the document. Programmers (like you, person reading this read-me!) often solve this using commenting -- methods that languages allow for text which is ignored / skipped by the interpreter, which in markdown's case means it won't be included in the final formatted product.

Markdown's use of formatting has been loosely defined for a while and wasn't part of its original definition, but Pandoc has settled on an option, at least. Code that is between two specific sequences of characters is 

The text you are reading is plain-text comments written within a commented out block the start of which is designated by a left-ward carat, followed by an exclamation point and two horizontal dashes (`<!--`). The end of which is designated by two dashes and an end colon > (). 
(I can't write the exact sequence here or else the comments block will end.). 
This text does not appear when the Markdown file is converted to HTML or PDF. 
Because commented text is ignored, you can delete these lines, leave them be, or even add additional comments throughout the document for your benefit.

## YAML Headers

The end of the syllabus header has a block which we call a YAML header. YAML, a recursive acronym short for 'YAML Ain't Markup Language', a *different* language from Markdown, mainly used for describing how data and text should be structured and developed as an alternative for XML. In Markdown documents, a 'YAML header' is a YAML formatted section which indicates information like title, author, and layout instructions usually 


is a section at the top enclosed by '---' lines, storing metadata like title or layout. This header helps in organizing content, setting parameters for processing the document, and is especially handy in static site generators where it can control page elements like navigation or appearance. 

designated by a line beginning with three repeated dashes (`---`) and ended by the same.


 and multiple YAML headers are allowed. 
This can be used to pass commands to pandoc that control the format of the resulting files. Within YAML blocks, comments are designated by lines that begin with hashes (#). 
Note that while pandoc will not render anything in a YAML header, some markdown previews in, for example, ghostwriter will render the YAML header.

##  Page Breaks

To create page break in the markdown for PDFs, just have a line that only contains the latex command "\newpage" . This command will not appear in HTML output when generated using Pandoc.
