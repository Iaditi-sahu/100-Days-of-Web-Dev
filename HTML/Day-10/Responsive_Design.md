# Responsive Design
** Responsive design is accomplished through CSS “media queries”. Think of media queries as a way to conditionally apply CSS rules. They tell the browser that it should ignore or apply certain rules depending on the user’s device.
** Media queries let us present the same HTML content as distinct CSS layouts. So, instead of maintaining one website for smartphones and an entirely unrelated site for laptops/desktops, we can use the same HTML markup (and web server) for both of them. 
** When you resize your browser, you should see three different background colors: blue when it’s greater than 960px wide, yellow when it’s between 401px and 960px, and red when it’s less than 400px.

Media queries always begin with the @media “at-rule” followed by some kind of conditional statement, and then some curly braces

** The only screen “media type” means that the contained styles should only be applied to devices with screens (opposed to printed documents, like when you hit Cmd+P in a browser). 
** A lot of these decisions are in the realm of design, which is outside the scope of this code-oriented tutorial; however, there are two concepts that you must understand as a developer:

   1. A “fluid” layout is one that stretches and shrinks to fill the width of the screen, just like the flexible boxes we covered a few chapters ago. 

    2. A “fixed-width” layout is the opposite: it has the same width regardless of the screen dimensions (we created one of these in the CSS Selectors chapter)
** Fluid layouts let us target a range of screen widths instead of specific mobile devices. This is very important for web designers. When they set out to create a mobile layout, they aren’t trying to make something that looks good on an iPhone 6s, Galaxy S7, or iPad mini—they’re designing a fluid layout that looks good anywhere between 300 pixels and 500 pixels (or whatever).

** In other words, the exact pixel values for the min-width and max-width parameters in a media query (collectively known as the “breakpoints” for a responsive website) don’t actually matter. Our website doesn’t care about the specific device the user is on. All it needs to know is that it should display a layout that looks pretty at 400 pixels wide (or whatever).

** It’s always a good idea to start with the mobile layout and work your way up to the desktop version. Desktop layouts are typically more complex than their mobile counterparts, and this “mobile-first” approach maximizes the amount of CSS that you can reuse across your layouts.