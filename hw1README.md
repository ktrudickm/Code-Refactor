# Homework Assignment 1 - Code Refactor

Marketing Agency - Site Accessibility Optimization

Problem: A marketing agency is looking to have their site optimized to both meet accessibility standards, and to also be fully optimized for search engines.


# HTML Accessibility Modifications & Findings

The first issue noticed was the Search Engine Optimization link at the top of the page did not direct the user to the respective spot on the page where that information existed when clicked. This was because the content it was trying to link to had an attribute that did not have an id called out, only a class. 

Another issue observed was that all of the images did not have alt attributes with them.

Continuing on, the structure of the HTML file was not clear. For example, the footer used a "div" attribute instead of a "footer" attribute. Also, the header was contained in the body, and was also under a "div" attribute and not a "header" attribute. Within the body itself, each section wasnt clearly distinguished since these sections were also under "div" attributes. So, it was adjusted from a "div" to a "section" and from a "div" to an "aside" to make it clear that each part of the site fit under a certian section of the page. The aside was fitting for the section that you see on the right-hand-side of the page since it is essentially "aside" of the main content to the left of it.


# CSS Accessibility Modifications & Findings

The css style sheet had multiple areas warranting improvement. There were redundant style classes created, just under different names. These were able to be consolidated into one based on what the style was trying to do. 

For example, for the "aside" attribute in the html, each individual section had its own class in the CSS file, even though they all had the same attributes:

                /* .benefit-lead {
                    margin-bottom: 32px;
                    color: #ffffff;
                }

                .benefit-brand {
                    margin-bottom: 32px;
                    color: #ffffff;
                }

                .benefit-cost {
                    margin-bottom: 32px;
                    color: #ffffff;
                } */

Instead, I created a class called .benefits section {} :

                .benefits section {
                    margin-bottom: 32px;
                    color: #ffffff;
                }

Because the parent attribute "aside" specified a class of benefits, and because benefits was already a class in the CSS, these three classes could be consolidated into one class since they each fell under the same parent attribute of "aside".

This was done for multiple classes within the CodeRefractor.css in order to consolidate and clean up everything so that the redundancy was eliminated. Below you can see the redundant styles commented out
and a general one created above it to encompass all three of them:


# Credits

The following resources were referenced during the project process:
W3Schools - [HTML Accessibility](https://www.w3schools.com/html/html_accessibility.asp "HTML Accessibility") <br/>
W3Schools - [HTML Attributes](https://www.w3schools.com/tags/ref_attributes.asp "HTML Attributes") <br/>
W3Schools - [CSS Toutorials](https://www.w3schools.com/css/default.asp "CSS Toutorials") <br>




