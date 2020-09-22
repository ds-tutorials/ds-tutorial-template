# Digital Scholarship Tutorial Template Info

## Introduction

Welcome to the Digital Scholarship tutorial template!

Now that your initial website is set up, these sample pages will walk you through everything you need to know to create your tutorial. Since you will not want to keep these pages, it is strongly recommended to bookmark the [template demo website](https://www.ds-tutorials.oucreate.com/tutorial-template/), where all of this information can be found.

Do not delete this page. Change the page title to the name of the tutorial and replace the contents with introductory information for learners. See the tutorial structure section for more information about what to include on the first page.

### Prerequisites

The tutorial website must first be setup using the Digital Scholarship Tutorial theme. Access to the theme repository and to the Digital Scholarship OU Create account is necessary for this step. See the [theme repository](https://github.com/TheoAcker12/digital-scholarship-tutorial) for more information.

!! If the repository link gives you a 404, you probably do not have access.

You will need to know how to use Grav (the basics) and how to write in Markdown. The required information will be provided in these pages.

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

## Grav

This will provide a brief overview of Grav that should be enough for working with the website. You can find additional information in the [official Grav documention](https://learn.getgrav.org/).

### The Admin Panel

The site dashboard can be accessed via the base site URL + `\admin`. You will need to log in using the OU DS tutorials username and password.

You may wish to go to Configuration -> Site to doublecheck the site title and the metadata description. These should already be set, but you can change them if needed.

#### Update Grav

Regularly update the website as needed. To check for updates, click the **Check for Updates** button on the top right of the admin panel dashboard.

1. If there is a new version of Grav, you can click **Update Grav Now** on the purple bar that will appear just below the updates button.
2. If themes or plugins have updates, you can click the **Update** button at the bottom right of the green Maintenance panel.
3. If there are no updates, you will see a message stating *Everything is up to date*.

### Plugins

The plugins page will provide a list of installed plugins. If needed, you can click on one of the plugins to access metadata (including a link to the readme) and configuration options. The following is a list of plugins that should/may be present. Additional information about a few plugins is provided below. Make sure to read everything in this section before making any changes.

- Admin Panel - provides the user interface you are currently using
- Admin Addon Media Rename - allows renaming images in the page editor
- Email - unnecessary, but automatically added
- Error - displays an error page when a requested page does not exist
- Form - unnecessary, but automatically added
- Google Analytics - supports gathering site usage statistics
- Git Sync - syncs page changes to a GitHub repository
- Grava11y (Accessibility for Grav) - optional, helps check for potential barriers to accessibility
- Highlight - provides syntax highlighting for code blocks
- Login - allows logging in to the admin panel
- Markdown Notices - adds markdown options
- Problems - detects and reports problems found in the site
- Shortcode Core - adds markdown options
- Shortcode UI - adds markdown options
- YouTube - optional, makes it easy to embed YouTube videos

It is also possible to add additional plugins, though this is unlikely to be necessary.

#### Git Sync

This is a very useful plugin as it syncs all of your page content each time you click *git* (Synchronize GitSync) on the left side of the admin panel just below the user name. Make sure to do this regularly, both so you have a backup in general and so that you can restore a previous version of a page if something goes wrong.

!! Avoid going to the Git Sync plugin configuration page itself. Every time you enter this page, it will fill out the *Git Password or Token* with something else. If you save at any time without changing this to the correct password first, future syncs will fail. Whenever you exit the page (even right after saving) you will need to continue without saving.

#### Highlight

This provides syntax highlighting for code blocks. If you are making use of it it is possible to change the color theme, but you need to make sure that the color contrasts are sufficient for accessibility.

#### Markdown and Shortcode Plugins

These plugins add possibilities to what you can do with Markdown, which will be included in the Markdown section.

### Themes

The themes page should include at least two themes - Digital Scholarship Tutorial and Learn2. Digital Scholarship Tutorial should be active.

The only thing you might want to do is click on Digital Scholarship Tutorial to access the configuration options and ensure that a URL has been provided for the GitHub repository where page content is being synced.

### Pages

#### Add and Edit Pages

You can easily add pages by using the three buttons at the top of the admin panel pages section (for page, chapter, or folder). You will specify the title of the page and whether the page belong on the top level or as the child of a folder.

The title is the first section in the editor, making it easy to change if you need to at any time (note that the title will be displayed above any content). If you do change the title, you may want to edit the folder and/or menu as described in the extra page options below.

Content is added in the Markdown editor provided, which invluded a preview button at the top right. The preview can help you check Markdown syntax, but keep in mind that the actual page will look somewhat different.

When you save your work, any changes will immediately be applied to the page in question, so you may want to keep the page open in another tab while you edit.

#### Add Media

When a page is saved for the first time, a folder and document will be created for the page. After that, you can add media by clicking on the box below the content editor. Hovering over an added image will provide an option to rename it at the bottom right. If you have a lot of images, you can reorder them by dragging and dropping.

Information on including images in the page can be found in the Markdown section.

#### Extra Page Options

The page editor *Content* tab is where you will spend most of your time, but you may want to set some options in the other tabs.

##### Options

The important areas on this tab are *Published* under **Publishing** and *Category* under **Taxonomies**.

A published page with a category of *docs* will be displayed as part of the tutorial. An unpublished page will not be reachable. A published page with a category other than *docs* will be visible in the side navigation but will not be included in the previous page/next page navigation, which should probably be avoided.

##### Advanced

###### Settings

When the page is created, the folder name will be the title in lowercase with spaces replaced by dashes. If the title is changed, the folder name will not change automatically. Keep in mind that the folder name will be displayed as part of the page URL and try to keep it short and descriptive.

If the page should be moved to the root (top level) or to be nested inside a folder, you can change the parent. The page template should be Chapter, Docs, or Folder.

###### Ordering

If it is not already, you can enable folder numeric prefix here. When enabled, you can drag and drop pages to sort them. This will determine page order in the navigation, and is important. When not enabled, pages will be sorted alphabetically.

###### Overrides

The menu is how the page will be displayed in the navigation. For example, the first chapter is listed as *Introduction* in the menu, although its folder name is *home* and its title should be the same as the title of the website. If the page title is very long, it may not fit well in the side navigation or the previous page/next page navigation, so modifying the menu may be useful.

If you want to remove the page from the navigation you can disable *Routable* and/or *Visible*.

##### Chapter Options

A subtitle can be provided for any chapter. The additional metadata options - lesson level, date updated, and created by - will only be used by the first chapter, as they describe the entire lesson.

##### Expert Mode

You may notice the ability to switch between normal and expert mode. It is advisable to always stay on normal mode - expert mode should not be necessary (or helpful).
