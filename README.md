# Ohmia Industry

Landing page for Ohmia Industry. Hosted on Github pages using the built in Jekyll processing.

## Structure and content

The landing-page is built up from different sections:
- Header (Logo and navigation)
- Hero (Title and lead text, with a background image)
- Illustration (Heading + image, used for displaying the diagram)
- Bullets (Icon + text, describing an unique selling point)
- Employees (Heading + optional text, list of employees with names, titles, and images)
- News (List of latest posts)
- Partners (Heading + optional text, list of logos)
- Footer (Contact information)

A post is composed of:
- Title
- Date
- Lead-text
- Optional background-image
- Content (markdown)

## Editing

### Text
The content of the landing-page is editable in the file "content.yml" which is placed in the root folder "_data". It is grouped by the respective sections, and stored as key-value pairs (key: "value"). The key is used to identify and place the content, while the value is the actual content. Only the value should be edited.

### Images
Images are stored under "assets/images" in a folder corresponding to the section. To change these images they can be either be replaced with a different file, or a new file can be uploaded and the filename updated in the "content.yml"-file.

### Employees and partners
To add employees or partners, duplicate the item (signified by the dash) edit the content, and upload an image with the correct filename to the respective folder. Important: The indentation must be the same.

### Footer
The information contained in the footer at the bottom is stored in the file "contact.yml" in the root folder "_data".


### Posts

Posts are stored in the folder "_posts". They are written in [Markdown](https://www.markdownguide.org/basic-syntax/).

To create a post, add a file to your _posts directory with the following filename-format:

> YEAR-MONTH-DAY-title.md

Where YEAR is a four-digit number, MONTH and DAY are both two-digit numbers. For example, the following are examples of valid post filenames:

> 2011-12-31-new-years-eve-is-awesome.md

> 2012-09-12-how-to-write-a-blog.md

To add a bakground-image and lead-text to the top of a post and on the card on the landing-page, the following must be added to the top of the file. Images must also be added to the "assets/images" folder.
>\---
>image: filename.jpg
>lead: Example lead text
>\---

To use local images, they must be uploaded to "assets/images" and linked in the post like this:

> \![Image caption]\(/assets/images/filename.jpg)
