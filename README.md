# Template Info

How to use the DS Tutorials Grav template once it is set up. 

Before following these instructions, make sure that a Digital Scholarship staff member has set up a Grav website using the Digital Scholarship Tutorial template. They will need a short title for the URL and the GitHub repository (e.g. grav, acrgis-storymaps-2020). Style rules: No capital letters, spaces, or special symbols. Only letters and numbers, with words separated by dashes.

You may want to at least read through the [Grav tutorial](https://www.ds-tutorials.oucreate.com/grav) and/or check out (some of) the [Grav documentation](https://learn.getgrav.org).

## Set Up

The tutorial will be hosted on: `https://www.ds-tutorials.oucreate.com/title` (replace title with the short title for the tutorial as mentioned above). You will want to open this page so you can view your changes as you work. You will work from the admin panel, which will be found at `https://www.ds-tutorials.oucreate.com/title/admin`. A Digital Scholarship staff member will provide the username and password needed to log in.

### Check for Updates

Click the **Check for Updates** button at the top right of the _Dashboard_. If there are any updates, install them.

### Change the Introduction

Go to the _Pages_ tab. The first page will be called _intro_. Click on this and go to the _Content_ tab. Replace the title with the title of the tutorial. This may be longer than the short title used in the URL. For example, _tableau-skyrim_ may become _Visualizing Data with Tableau_.

Then go to _Chapter Options_. Add a subtitle to serve as a brief description of the tutorial, choose the lesson level, and enter the date and your name. Remember to save when you're finished!

### Starting Pages

The pages/folders _examples_ and _presentations_ have been included as an example of what you can do. You will want to delete these when you no longer need them.

## Adding Pages

To add a page, choose the **Add Documentation Page** button on the _Pages_ tab. Give the page a title and set the parent page as the chapter that the page belongs to. (If you aren't using chapters, the parent page will always be _/intro_). On the _Advanced_ tab for the new page make sure that **Folder Numeric Prefix** is Enabled. This last step is only necessary for the first page you add to a chapter. When adding additional pages to that chapter, Grav will recognize that the other pages for that chapter have numeric prefixes and will automatically add it to any new ones.

For information about adding content and media, please see the [Grav documentation](https://learn.getgrav.org) or the [DS Grav tutorial](https://www.ds-tutorials.oucreate.com/grav) (also mentioned above).

## Adding Chapters

To add a chapter, choose the **Add Chapter** button on the _Pages_ tab. Under _Chapter Options_ you may want to give it a subtitle, but this is optional. You will want to make sure the page is not listed as an introduction.

## Markdown Options

Beyond the default markdown options, Grav has a number of fancy options added by a couple of plugins. Look for _Markdown Notices_ and the "shortcode" plugins (_Shortcode Core_ and _Shortcode UI_) on the _Plugins_ panel and view their readmes for more information.

In markdown a piece of in-line code is marked with the \` mark on either side. A block of code begins with three of these (you can find more information in Grav's [markdown documentation](https://learn.getgrav.org/16/content/markdown). What is important here is that the template allows you to add a clipboard icon to any code section, which readers can use to easily copy the code. To use this feature, your inline code must look like: `` `CLIP: code here` `` and your block of code must look like:

~~~md
```
CLIP: code here
more code
more code
```
~~~

Adding "CLIP: " to the start of your code is very important.

## Resizing Images (and more)

If you want to resize an image you can add `?cropResize=width,height` to the end of your image URL. You must provide both numbers, but cropResize will scale the image so that it fits within the box you have specified but does not necessarily fill that box. (It will also cut off any empty space, so if you are resizing an image with the original dimensions of 400,400, `?cropResize=100,1000` and `?cropResize=200,100` should have no difference. This is the most likely function you will want to use, but the [Grav documentation](https://learn.getgrav.org/16/content/media) has information on a number of other functions.

Example usage for an image named `my-image.png` within the folder of the page you are displaying it: `![alt text](my-image.png?cropResize=300,300)`

## Updating

Remember to change the date of last update on the first (intro) page. If you are updating a work that someone else has written, check for policy of how to write authors.
