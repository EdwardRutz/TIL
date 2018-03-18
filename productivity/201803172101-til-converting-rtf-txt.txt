# TextUtil: Convert Text Files From One Type to Another

#til
Author: er

## Intro

TextUtil quickly converts almost any text format to another format.
This is a command line tool to use in terminal and appeared in OS X 10.4.
- Convert *.txt files to *.html files
- Convert *.rtf files to *.docx files
- Convert *.docx files to *.txt files

## Why this is Important

- Be software agnostic
- Moving files outside an app that has them locked up
- Future proofing you work
- Convert files to HTML to use in websites

## Step-By-Step

- Simply open terminal, move into the directory with the files you want to change and type the textutil commands
- Or if you prefer, instead of navigating to the folder type the command in the terminal and add  the file path of the files you want to convert to your textutil command

### Examples

```
//Convert RTF to TXT:
 textutil -convert txt /path/to/DOCX/files/*.rtf
 
//or navigate inside the directory and type: 
  textutil -convert txt *.rtf

//Convert DOCX to TXT:
textutil -convert txt /path/to/DOCX/files/*.docx

//Convert TXT to DOCX
- Navigate inside the directory and type:
textutil -convert docx *.txt

//Convert DOCX to RTF :
textutil -convert rtf /path/to/docx/files/*.docx

//Convert TXT to HTML
 textutil -convert html *.txt 
```

## TL;DR



## References

- Notes: [[201803171808-convert-rtf-to-txt]]