# peoples-roman-history notes

Ancient map tiles,
https://cawm.lib.uiowa.edu/index.html

## Convert DOCX to MD

Students submit essays in DOCX form in OneDrive. 

Clean up essays in DOCX, then use pandoc to convert to markdown:

`for f in *.docx; do pandoc -f docx -t gfm --wrap=none -o "${f%.docx}.md" "$f"; done`
