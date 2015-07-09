BOOTSTRAP STYLEGUIDE
==============================

A starting point for crafting living style guides for Bootstrap-based projects.

Based on Brett Jankord's [Style Guide Boilerplate](http://brettjankord.com/projects/style-guide-boilerplate/)

[Read More about the project](http://www.google.com/‎)

[Demo](http://www.google.com/)

*Note: Sample patterns have been included in the demo. Your site will have it's own unique patterns.*

![Bear vs wolf](http://i.ytimg.com/vi/SrXGUybN_Qw/hqdefault.jpg)

## Getting Started With Style Guide Boilerplate

### Download the Style Guide Boilerplate
You can clone, fork, or download the repo from GitHub.
Once you have the files for **Style Guide Boilerplate**, you'll create a directory on your site for them.

### Set up your project name
Open the `index.php` file, and look for line 2, where it says:
`$project_name = "Project";`
Put your own project name between the quotation marks

### Hook up your own CSS into the style guide
In the `<head>` of **Style Guide Boilerplate** are custom styles for the boilerplate itself. These have all been prefixed with sg- so they hopefully shouldn't cause any conflicts with your website's own styles. You need to compile the styleguide.less file with your bootstrap variables.less file and mixins

Below the custom styles for the boilerplate, you will add in your own custom stylesheet(s) which you use on your live site.


    <!-- Replace below stylesheet with your own stylesheet -->
  	<link rel="stylesheet" href="css/sub-theme.css">


### Set up a directory on your site for the style guide
I recommend creating a directory named `style-guide` in your site's root directory. I think it would be awesome if I could go to `anysite.com/style-guide/` and check out that site's style guide.


### Review your live site CSS
You should be able to go to `yoursite.com/style-guide/` and see how your live site's CSS affects base elements.
The last step is creating your sites custom patterns/modules.

### Create custom documentation files
You can create an intro or other documentation files. Just create an html file with the contents, styled in html, and upload the file as `document-title.html` into the `docs` directory inside of your `style-guide` directory.

### Configure foundation elements
The boilerplate comes, by default, with guides for **colors, typography**, and a visible bootstrap basic **grid**. You can edit these or add new ones for things such as textures, icons or imagery, also by creating an html file and uploading to the `foundation` dir.

#### Setting up color swatches
The sample file comes with the bootstrap primary and brand colors pre-configured. But to include the ones in _your_ bootstrap theme, you can use the styleguide.less file included in this package. It is set up to import your bootstrap variables, and when compiled, will generate the appropriate swatches. Make sure the import path at the top of the file is correct before compiling. If you need more colors, feel free to add more classes to the .less file.

#### Setting up font stacks
The boilerplate comes, likewise, with predefined classes for primary and secondary Bootstrap font-family declarations

### Create custom base styles patterns
The boilerplate comes with many bootstrap elements built in, such as buttons, breadcrumbs, alert messages, etc., but you can customize them by adding, deleting or modifying the files within the `markup/` directory
Save the file as `pattern-name.html` into the `markup/patterns` directory inside of your `style-guide` directory.

You should now be able to see the new patterns at `yoursite.com/style-guide/`


###Create Usage documentation

To create personalized usage documentation for your markup examples, create a new .html file and name it whatever your markup snippet is named.

Save the file as markup-name.html into the usage/base or usage/patterns directory inside of your style-guide directory.

For example, if you want to create doc for markup/patterns/breadcrumbs.html, create a file called breadcrumbs.html and save it into usage/patterns.

You should now be able to see the new doc at `yoursite.com/style-guide/`.
