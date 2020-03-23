# Template Info

How to use the DS Tutorials Grav template once it is set up. Before following these instructions, make sure that a Digital Scholarship staff member has set up a Grav website using the Digital Scholarship Tutorial template. They will need a short title for the URL and the GitHub repository (e.g. grav, acrgis-storymaps-2020). Style rules: No capital letters, spaces, or special symbols. Only letters and numbers, with words separated by dashes.

## Set Up

The tutorial will be hosted on: https://www.ds-tutorials.oucreate.com/title (replace title with the short title for the tutorial as mentioned above). You will want to open this page so you can view your changes as you work. You will work from the admin panel, which will be found at https://www.ds-tutorials.oucreate.com/title/admin. A Digital Scholarship staff member will provide the username and password needed to log in.

### Check for Updates

Click the _Check for Updates_ button at the top right of the Dashboard. If there are any updates, install them.

### Change the Introduction

Go to the Pages tab. The first page will be called intro. Click on this and go to the Content tab. Replace the title with the title of the tutorial. This may be longer than the short title used in the URL. For example, tableau-skyrim may become Visualizing Data with Tableau.

Then go to Chapter Options. Add a subtitle to serve as a brief description of the tutorial, choose the lesson level, and enter the date and your name. Remember to save when you're finished!

### Starting Pages

Examples and presentations pages have been included as an example of what you can do. You will want to delete these when you no longer need them.

## Adding Pages

To add a page, choose the Add Documentation Page button on the Pages tab. Give the page a title and set the parent page as the chapter that the page belongs to. (If you aren't using chapters, the parent page will always be /intro). On the Advanced tab for the new page make sure that Folder Numeric Prefix is Enabled.

For information about adding content and media, please see the Grav documentation or the DS Grav tutorial.

## Adding Chapters

To add a chapter, choose the Add Chapter button on the Pages tab. Under Chapter Options you may want to give it a subtitle, but this is optional. You will want to make sure the page is not listed as an introduction.

## Markdown Options

Beyond the default markdown options, Grav has a number of fancy options added by a couple of plugins. Look for the "shortcode" plugins on the Plugins panel and view their readmes for more information.

In markdown a piece of in-line code is marked with the \` mark on either side. A block of code begins with three of these (you can find more information in Grav's markdown documentation. What is important here is that the template allows you to add a clipboard icon to any code section, which readers can use to easily copy the code. To use this feature, your inline code must look like: `` `CLIP: code here` `` and your block of code must look like:

~~~md
```
CLIP: code here
more code
more code
```
~~~

Adding "CLIP: " to the start of your code is very important.

## Updating

Remember to change the date of last update on the first (intro) page. If you are updating a work that someone else has written, check for policy of how to write authors.
