# Peoples' Roman History Template

Students submit essays to the project in three parts:

1. **Google Doc** -- contains the content of your essay, following a set of basic conventions.
2. **Google Sheet** -- *if you are using images or other items in your essay*, you will create a Google Sheet that lists and describes each of the items you want to include with your essay, along with their associated metadata. 
3. **Google Form submission** -- you will submit a Google Form providing metadata about your essay topic and the share links to your Doc and Sheet.

The requirements for these submissions is described in the public facing docs pages, /project/essay.html

## Data

These submissions become the project data in two parts:

- "peoples-roman-history.csv" - the main metadata file that generates entries across the site. 
    - The parent entries are created from the Google Form submissions. They contain the structured data about each entry.
    - Child entries are created from all the submitted Google Sheets containing media records.
    - The two Sheets tables are prepped, then combined with OpenRefine.
- markdown files in "_essays/" - Each submitted Google Doc is converted into a markdown file and cleaned up following the conventions.

## Customizations

- "_layouts/item/essay.html" - the base item layout for entries.
- "_essays/" - the jekyll collection of essay content. These files do not generate a page. They are called into the essay layout.
- "_includes/essay/" - customized includes for use in the essay content. These pull data from the media csv rather than main metadata.
