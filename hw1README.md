# Homework1
Homework Assignment 1 - Code Refactor

Marketing Agency - Site Accessibility Optimization

Problem: A marketing agency is looking to have their site optimized to both meet accessibility standards, and to also be fully optimized for search engines.


HTML Accessibility Modifications & Findings

The first issue noticed was the Search Engine Optimization link at the top of the page did not direct the user to the respective spot on the page where that information existed when clicked. This was because the content it was trying to link to did not have an id called out, only a class. 

Another issue observed was that all of the images did not have alt attributes with them.

Continuing on, the structure of the HTML file was not clear. For example, the footer used a <div> instead of a <footer>. Also, the header was contained in the body, and was also under a <div> and not a <header>. I also adjusted the <body> to <main> since the main content was less of a body, than it was the main content of the page. WIthin the main itself, each section wasnt clearly distinguished since these sections were also under <div>'s. So, it was adjusted from a <div> to a <section> to make it clear that each part of the site fit under a certiansection of the page.


CSS Accessibility Modifications & Findings

The css style sheet had multiple areas warranting improvement. There were redundant styles created, just under different names. These were able to be consolidated into one based on what the style was trying to do. 