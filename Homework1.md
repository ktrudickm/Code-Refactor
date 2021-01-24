# Homework1
Homework Assignment 1 - Code Refactor

Marketing Agency - Site Accessibility Optimization

Problem: A marketing agency is looking to have their site optimized to both meet accessibility standards, and to also be fully optimized for search engines.

When diving into the style.css file for the site, you can see that there are multiple classes defined for the same thing. Here, there is a class .footer and a class .footer h2: 

/var/folders/lt/1vs80bdn5hb2zwqyg3npmcy00000gn/T/TemporaryItems/NSIRD_screencaptureui_o9bIKU/Screen Shot 2021-01-20 at 8.51.00 PM.png

This is redundant, since the .footer h2 contents (font-size) can just be placed in the .footer class.
This same thing occured throughout the entire style.css file for almost all of the classes defined.
