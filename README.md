# Digital Scholarship Tutorial Template Info

## Introduction

Welcome to the Digital Scholarship tutorial template!

Now that your initial website is set up, these sample pages will walk you through everything you need to know to create your tutorial. Since you will not want to keep these pages, it is strongly recommended to bookmark the [template demo website](https://www.ds-tutorials.oucreate.com/tutorial-template/), where all of this information can be found.

Do not delete this page. Change the page title to the name of the tutorial and replace the contents with introductory information for learners. See the tutorial structure section for more information about what to include on the first page.

### Prerequisites

The tutorial website must first be setup using the Digital Scholarship Tutorial theme. Access to the theme repository and to the Digital Scholarship OU Create account is necessary for this step. See the [theme repository](url) for more information.

!! If the repository link gives you a 404, you probably do not have access.

You will need to know how to use Grav (the basics) and how to write in Markdown. The required information will be provided in these pages.

How to use the DS Tutorials Grav template once it is set up. To set up, you must have access to the [tutorial template repository](https://github.com/TheoAcker12/digital-scholarship-tutorial) (If you receive a 404 error, that is because you do not have access to it).

Before following these instructions, make sure that a Digital Scholarship staff member has set up a Grav website using the Digital Scholarship Tutorial template. They will need a short title for the URL and the GitHub repository (e.g. grav, acrgis-storymaps-2020). Style rules: No capital letters, spaces, or special symbols. Only letters and numbers, with words separated by dashes.

You may want to at least read through the [Grav tutorial](https://www.ds-tutorials.oucreate.com/grav) and/or check out (some of) the [Grav documentation](https://learn.getgrav.org).

## Tutorial Structure

### First Chapter

The first chapter requires special configuration, so be sure not to delete the provided sample page. Instead, edit the page and replace the current title and content as follows:

1. The title of the first chapter should be the same as the title of the tutorial/website.
2. In *Chapter Options*, the subtitle should provide a brief description of the tutorial.
3. In *Chapter Options*, the three pieces of metadata should be set (and updated later as needed) - lesson level, last updated, and created by.
4. The page contents should include
	1. A brief explanation of the tutorial contents and if possible an example of the finished product
	2. Any previous knowledge or experience required
	3. Any useful reference materials
	4. Setup instructions for downloading data, installing software, etc.

If the first page is missing for any reason, you can manually edit the header in expert mode to include the line `isIntro: true`.

### Folder Structure

You can nest chapters and pages inside folders if the tutorial requires additional structure. Be aware that a page should never serve as a folder/container for another page. Such a page will become inaccessible from the main navigation and may cause issues with the previous/next navigation.

The admin panel includes an *Add Folder* button in the Pages section for this purpose. Using this button will automatically create a folder that is visible but not routable. In general, as long as folders are visible but not routable, they should function as needed.

### Chapters and Pages

The contents of the tutorial will exist in normal pages (docs) or chapters. Chapters mark the beginning of a new section of content and will typically be the first page within a top level folder.

- Chapters will have the option to include a subtitle.
- The additional metadata (lesson level, etc.) in *Chapter Options* will be ignored by all but the first chapter.
- All pages to include in the tutorial must have *Category* set to *docs*. This should happen automatically when creating a new docs or chapter page.

