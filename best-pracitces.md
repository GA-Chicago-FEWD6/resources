#Best Practices

##File Handling

- Files and folder names should not contain odd characters like spaces " " — instead use dashes (-) or underscores (_)
- Files and folder names should be written in all lower-case (about-me.html not About-Me.html)

##HTML

- Always indent nested elements with 2-space tabs
- Close tags immediately after you open them so you don't forget later
- Nothing should be naked — all text should be wrapped in an HTML tag
- Elements that don't contain immediately nested elements should be written on a single line (example)
- Keep project folders organized — the index.html should be in the root directory, images etc should be in sub-directories named as such
- Always add an "alt" attribute to your `<img>` tag that describes that image (ex: `<img src="flag.png" alt="The Chilean National Flag">`)
- Always opt for the more semantic HTML5 tags instead of plain `<div>`s when appropriate

##CSS

- Format CSS declarations with each property on a new line, indented with 2-space tabs (ex: http://d.pr/i/17ISs)
- Avoid being super specific with your CSS declarations, and avoid using `!important` completely
- Don't use the universal selector (`*`) to declare global styles, instead declare them on the body element (`body`)
- Try and write your CSS declarations from the most generic declarations (body, class-less elements), to the most specific (classes, ids, specific sections/pages) from top-to-bottom
- Order your CSS properties however you like (https://css-tricks.com/poll-results-how-do-you-order-your-css-properties/) but make a concious choice and stay consistent with how you order them
- For easier layout in CSS apply `box-sizing: border-box;` via the recommended method: http://www.paulirish.com/2012/box-sizing-border-box-ftw/
- Be wary of creating classes or ID names similar to names used by CSS and HTML e.g. a class named `body` or `float`

##JavaScript

- When possible, start out by planning your program, and write pseudo code to layout the tasks of your program
- Always place your JavaScript in an external .js file, and place the reference to that file just before the closing </body> tag, rather than in the <head>
- Variables and function names should be written in camel case (ex: `myFunction(); var firstVar;`)
- Keep style changes out of JavaScript whenever possible, instead when you need to trigger style changes via JavaScript, add and remove new classes that can then be styled in CSS
- Leave comments (`// like this`) to explain anything that might need clarification
Each statement should begin on a new line, and each statement should end with a semicolon (";")
When working with your JavaScript, use methods like `alert();` and `console.log()` to give yourself messages in the dev tools console to help figure out if your functions are running properly or not
Whenever possible, use jQuery to add or remove CSS classes to handle changes in design rather than relying on jQuery methods like `.slideToggle()`, `.show()`, or `.hide()`, as they are much heavier and less flexible than using CSS classes to handle these changes