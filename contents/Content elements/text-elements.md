Page: Content Elements | Text elements
=============

# Text elements

You use text elements to include different types of text content on your page. 
Contao offers special elements that are optimized for management in the back-end and deliver correct output in the front end. In the following paragraphs the characteristics of the individual element types are described and explained.

## Headline

The headline element adds a single headline to your page. You can set the level of the headline ranging from h1 to h6.

The first headline on this page was created by using a headline element with the level set to h1.

But you do not have to use this element to add a headline to your page. Almost every other element features an additional input field to add a headline also offering the levels h1 to h6.

## Text

The text element provides a rich text editor in the back-end allowing you to format the text output in the same way as popular office software. You can set words or phrases in bold or italic or add underlining and integrate (hyper) links to other pages of the same website, links to files or file downloads or external URLs to name just a few features of the utilized tinyMCE editor.

The element also allows to add a single image which can be positioned relatively to the text. The image can be placed above or below the text or placed floating left or right of the text. You are able to choose from several options to modify the picture, e.g. resizing or even cropping it and to add a link to a contao page, to an external URI or to a full resolution version of the image. You can define wether the linked page will be opened in a new window or tab of your browser. The full resolution version of the image will be opened in an overlay on the same page if defined that way in the page layout.

## HTML

The HTML element can be used to enter pure HTML code.

The allowed tags have to be defined in the contao settings in the security section. Most of the HTML tags are allowed by default. Some tags with security relevance such as 'script' have to be added manually if needed.

### Definition list Example
<dl>
  <dt>Buil with the Contao Content Element HTML.</dt>
  <dd>You can use many more HTML Tags if you like.</dd>
</dl>

## List

To add ordered or unordered lists as a single element - not within the text element - contao provides the list element. With a special back-end widget you can add each list entry via a single input field, sort the entries, insert new entries or copy them.

### ORDERED LIST EXAMPLE

* Ordered List Example 1
* Ordered List Example 2
* Ordered List Example 3
* Ordered List Example 4

### UNORDERED LIST EXAMPLE

1. Unordered List Example 1
1. Unordered List Example 2
1. Unordered List Example 3
1. Unordered List Example 4

## Table

To create a table you can use the table element. Contao offers a special back-end widget, similar to the one utilized for lists, to add columns and rows, define a head- and footer-row and add a summary for the table content. In the front-end output, special classes can be chosen and added to the table, rows and cells. Just check the HTML code of the page content elements, to explore the possible classes.

In addition, you can add a sorting option for the frontend to make the table sortable by all columns.

### EXAMPLE

| Head 1 | Head 2 | Head 3 |
|--------|--------|--------|
| Column 1 | Column 2 | Column 3 |
| Column 1 | Column 2 | Column 3 |
| Column 1 | Column 2 | Column 3 |

## Code

To provide a snippet of programming code like i.e. Php or JavaScript, you use the code element. The code will not be executed in the front-end of the page.

```
<script>
  alert('Hello World!!');
</script>
````
