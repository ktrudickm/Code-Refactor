# Homework Assignment 1 - Code Refactor

Marketing Agency - Site Accessibility Optimization

Problem: A marketing agency is looking to have their site optimized to both meet accessibility standards, and to also be fully optimized for search engines.


## HTML Accessibility Modifications & Findings

The first issue noticed was the Search Engine Optimization link at the top of the page did not direct the user to the respective spot on the page where that information existed when clicked. This was because the content it was trying to link to had an attribute that did not have an id called out, only a class. 

Another issue observed was that all of the images did not have alt attributes with them.

Continuing on, the structure of the HTML file was not clear. For example, the footer used a "div" attribute instead of a "footer" attribute. Also, the header was contained in the body, and was also under a "div" attribute and not a "header" attribute. Within the body itself, each section wasnt clearly distinguished since these sections were also under "div" attributes. So, it was adjusted from a "div" to a "section" and from a "div" to an "aside" to make it clear that each part of the site fit under a certain section of the page. The aside was fitting for the section that you see on the right-hand-side of the page since it is essentially "aside" of the main content to the left of it.

See below for the before/after of the header, body, and body elements, respectively:

### Header content before:
![header-before](./Assets/images/headerbefore.png =150px)

### Header content after:
![header-after](./Assets/images/headerafter.png =150px)

Above in the before, you can see that the header is in the body and it has a div attribute as opposed to a header attribute. In the after, the header is under a header attribute and is before the body.

### Body content before:
![body-before](./Assets/images/bodyafter.png =150px)

### Body content after:
![body-after](./Assets/images/bodyafter.png =150px)

You can see in the above screenshots that before the html was cleaned up, almost everything is under a div attribute, making it confusing as to what the content really is in relation to the page. The after screenshot shows this issue cleaned up to make the portion being shown under the attribute of main, since it is the main content of the page, and then each item within the main attribute, is under a section attribute since they are each different sections within the main content.

### Footer content before: 
![footer-before](./Assets/images/footerafter.png =150px)

### Footer content after:
![footer-after](./Assets/images/footerafter.png =150px)

The footer before is under a div attribute. In order to make this meet accessibility standards and to make it more readable/understandable to the reader, the div was changed to a footer attribute, which you can see in the after photo.

## CSS Accessibility Modifications & Findings

The css style sheet had multiple areas warranting improvement. There were redundant style classes created, just under different names. These were able to be consolidated into one based on what the style was trying to do. 

For example, for the "aside" attribute in the html, each individual section had its own class in the CSS file, even though they all had the same attributes. See below for the changes made, and note that the commented out classes were the original redundant ones, with the benefits section being the updated one:

![class-consolidating](./Assets/images/class-consolidating.png =150px)

Because the parent attribute "aside" specified a class of benefits, and because benefits was already a class in the CSS, these three classes could be consolidated into one class since they each fell under the same parent attribute of "aside" under the attribute of "section":

![html aside](./Assets/images/aside.png =150px)

This was done for multiple classes within the CodeRefractor.css in order to consolidate and clean up everything so that the redundancy was eliminated. Below you can see the redundant styles commented out
and a general one created above it to encompass all three of them:


## Credits

* The following resources were referenced during the project process: 
* W3Schools - [HTML Accessibility](https://www.w3schools.com/html/html_accessibility.asp "HTML Accessibility") 
* W3Schools - [HTML Attributes](https://www.w3schools.com/tags/ref_attributes.asp "HTML Attributes") 
* W3Schools - [CSS Toutorials](https://www.w3schools.com/css/default.asp "CSS Toutorials")




