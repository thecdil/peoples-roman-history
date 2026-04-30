# Prep Essay Submissions

## Student Edit Needs

Students should work on-->

In essays:

- Front matter (title, email, author)
- Don't repeat structured information
- Headings formatting
- Replacing images with objectid convention, ensuring it matches the media spreadsheet

In media spreadsheet:

- no hyperlinks in cells (full URL needed)
- review your "source", it should look like a formal citation

In data:

- title = character name
- review time periods (CE, shorter ten - twenty years)
- review locations (provinces!)
- consistency overall! 

https://thecdil.github.io/peoples-roman-history/project/essay.html

## Editor Process

In the "peoples-roman-history_combined" Sheet:

- On the "essays" tab, select a record. Click the "doc_link" and "sheet_link" to see submissions.
- Review the media sheet at the "sheet_link". Copy the rows over to the "media_combined1" tab of "peoples-roman-history_combined".
    - ensure the "objectid" are filled in, unique, logical. 
    - fill in the "essayid" column with the essay's objectid
- Click the "doc_link" and download the essay as a DOCX (File > Download > DOCX). Rename the file by objectid.

### Convert DOCX to Markdown

- Place all downloaded essay files into a folder
- Open terminal in the folder
- Use this pandoc command: `for f in *.docx; do pandoc -f docx -t gfm --wrap=none -o "${f%.docx}.md" "$f"; done`
- Copy the .md files into the "_essays/" folder

### Prep Essay Markdown

First, fix up the front matter at the top.
It must look like:

```
---
title:
author:
---
```

This will require wrangling because it doesn't come down clean from GDocs. 
Note: we asked for author_email, but delete the email before committing to the project! 
The title and author is often included as a heading/content--add to the front matter and delete from the essay body.
Watch for titles with colons, they need to be quoted to avoid breaking YAML!

Second, fix up any images to use the essay/image.html include.
Each image should look like:

`{% include essay/image.html objectid="test-img-01" %}`

If the author provided a caption, you can add a caption option to the include (be careful of quoting! Also note, captions can not have markdown formatting).

`{% include essay/image.html objectid="priest001" caption="Figure 1 - Image showing a possible route for the Augustan aqueduct." %}`

Polishing:

- Delete character structured data (that should be in the spreadsheet)
- Clean up headings
    - normalize hierarchy starting at level two
    - remove extra bold `**` formatting if necessary
    - make random bolded sections into proper headings if necessary
- Clean up white space
- Delete any extra html markup
- "Sources" should be a heading `## Sources`
- Sources should be a list (`- `, not a blockquote `> `). Unfortunately sources formatting tends to be a mess!
- Check against original file

If there are footnotes, the correct formatting looks like:

```
In text citation.[^1]

[^1]: Please note this is a note.
```
