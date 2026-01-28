---
title: Contributing
permalink: /project/essay.html
layout: page-narrow
---

# Contributing to the Project

Each student or team of students will contribute one exhibit page to this digital project. 
Each entry is created from three parts:

1. **Google Doc** -- contains the content of your essay, following a set of basic conventions.
2. **Google Sheet** -- *if you are using images or other items in your essay*, you will create a Google Sheet that lists and describes each of the items you want to include with your essay, along with their associated metadata. 
3. **Google Form submission** -- you will submit a Google Form providing metadata about your essay topic and the share links to your Doc and Sheet.

Details for completing each part is described below.

----------

## Essay Document

To get started, create a copy of the essay template in Google Docs:

[Create Copy Essay Project Template](https://docs.google.com/document/d/1eQeySiAK-4O-e6Ym5lIRsNloiFa6IFg15qdthnaFLwo/copy){:.btn .btn-lg .btn-success}

Once you have your copy, rename your file using this pattern `lastname_firstname_doc` (e.g. "williamson_evan_doc").

### Front Matter 

At the top of the Doc you will find some front matter that looks something like:

—<br>
Title: [name of the essay, will appear at top of the essay]<br>
Author_email: [your uidaho email(s), this is for internal use–it will not be in the website!]<br>
Author: [your name(s) as you want it to appear on the website]<br>
—<br>

Fill in the structured information, following the instructions in square brackets (and delete the instructions!). 

Below the front matter you see some instructions about how to add your content for the three essay options:

- Narrative essay: write your essay in this document using properly formatted headings and footnotes.
- Video essay: please upload your project to a service such as YouTube or Vimeo, then paste the link to your video below. Provide any text that will be displayed with the video on your exhibit page.
- Multi-modal essay: write your text in this document. Create a copy of the media_information_template Sheet. List and document your images and media in the Sheet. 

Delete the instructions and start writing following the conventions below!

### Formatting 

Try to keep any formatting simple since this content will become a webpage where text reflows to many different screen sizes--any complex formatting or layout in the Doc will be stripped away when converting into data (Markdown) for the project.
Feel free to use inline styles such as _italics_ and **bold**, and block styles such as lists and block quotes.

Use Insert > Page elements > Footnote to add footnotes to your content.

### Headings

When reading on the web, users expect more headings and smaller blocks of text than a typical academic essay.
You will want to use plenty of meaningful headings (those bolded phrases breaking up the text like "Headings" above this line). 

They function to help people navigate and understand your content--think of them like a table of contents, dividing the text into logical sections and sub-sections.

To apply headings in your Google Doc, select the text that should be a heading, then in the menu ribbon above, select the dropdown that says "Normal text" and change it to "Heading 1", "Heading 2", etc. 
Your headings are _hierarchical_ and should follow in logical order, starting from "Heading 1" and increasing sequentially (with out skipping levels) for sub-topics.
When you start a new topic, you can jump back up the levels to reflect the structure of your content.

### Images and Media 

Rather than pasting images or other media directly into your document, you will use a basic convention. 

First, you will fill in the individual image's information in your Item metadata spreadsheet (details in the next section). 
Then, in the location in your text where you would like images or other media to appear, add a blank line, then put: 

`[objectid: exampleid]` 

where "exampleid" matches the id from your item metadata spreadsheet. 

When your essay is converted into data for the website project, this convention will pull in the information from your metadata spreadsheet to add the image to the web page. 
This ensures that each media Item is fully documented as a source and correctly formatted for the web.

For example, using the convention in your Doc might look like:

`[objectid: example01]`

on the final website, that convention will be replaced by the actual image, something like:

{% include feature/image.html objectid="test-img-01"  %}

----------

## Media Item Sheet

*If you are using images or other media items in your essay*, you will create a Google Sheet that lists and describes each of the items you want to include with your essay, along with their associated metadata. 
To get started, create a copy of the Sheet template in Google Docs:

[Create Copy Media Information Template](https://docs.google.com/spreadsheets/d/1Sfn-fz5k1J8bGOVa6LiF9-NFD7kN1NFkqvkIcX4a7tw/edit?usp=copy){:.btn .btn-lg .btn-primary}

Once you have your copy, rename your file using this pattern `lastname_firstname_sheet` (e.g. "williamson_evan_sheet").

In this spreadsheet you will describe each image or other media.
Each row represents one image. 
The columns represent structured information (metadata) about each item.

For each item you will provide:

- **objectid** - a unique id for the item so it can be referenced in the project. Create an id following the pattern `lastname001`. e.g. "williamson001", "williamson002", etc.
- **title** - The name or label given to the digital object. What is the Item called?
- **description** - a short explanation of the item and significance. e.g. "Photograph showing downtown Spokane after the 1889 fire."
- **source** - A clear citation to where the item comes from, i.e. the physical or digital source of the item. e.g. "Map of Bovill, Idaho Cities and Towns Collection, University of Idaho Library Digital Collections, https://www.lib.uidaho.edu/digital/cities/items/cities1083.html"
- **original_link** - the URL to the web page where the item can be found
- **link_to_media** - the direct link to the image or media download if possible
- **image_alt_text** - Concise, descriptive text conveying visual content for accessibility

*Note:* if you have scanned or photographed items yourself, please upload and share the files via OneDrive or Google Drive. 
Provide the link in the "link_to_media" column.

----------

## Submission Form

To submit your essay, you will use a Google Form providing metadata about your essay topic and the share links to your Document and Sheet. 

**The submission form link will be available in Canvas.**

### Prep

Once your essay Doc and Sheet is complete, carefully check over the formatting, filename, and record details to ensure everything is correct. 

Then, go into your essay Doc and Sheet, and enable sharing:

- Select "File" > "Share"
- Under "General Access", choose "Anyone with the link"
- Select "Commenter"
- Then "Copy link" to get the full url.

### Metadata 

The metadata represents the standardized fields we will all use to describe the exhibits and the historical characters you created. 
They allow users to discover, browse, and understand the essays.

The instructor provided you the seeds of this information, which you will have full fleshed out by the time you submit this form. 

The form will ask you:

- Title - The name of your character, or title of your essay. Will appear at the top of the web page and browsing features
- Essay type - Narrative, Multi-modal Essay, or Video
- Description - A short description of your essay content or character profile
- Time period - The time period your essay covers
- Location - The main location of your essay or character profile
- Province - The Roman province where it is located
- latitude - Use [Pleiades gazetteer](https://pleiades.stoa.org/) or other historical source to find appropriate lat/long for the location of your character's story
- longitude 
- status - Citizenship status in the Roman Empire
- gender - Character's gender
- age - character's age
- occupation - character's occupation
- family status - Describe character's family status
- themes - choose the main historical topics your essay explores from the course list, or add your own:
    - race/ethnicity
    - gender
    - sexuality
    - labor
    - inequality
    - spectacle
    - violence
    - life stages (birth, childhood, motherhood, marriage, childbearing, coming of age, death, etc.)
    - empire
    - slavery
    - class
    - bodies/regulation/law
    - masculinity
    - identity
    - citizenship
    - travel/mobility
    - religion and magic
    - Othering and difference
    - Orientalism
    - Cultural exchange
    - Imperial language/propaganda
    - Cultural reception (what I’m calling “Roman Afterlives”)
- author - The name(s) of authors of this essay, as you want them to appear on the website
- essay Google Doc link 
- Item Google Sheet link 
- featured image objectid - If you submitted a Google Sheet and have one image that should be featured to represent your essay, please paste the objectid of the item here
