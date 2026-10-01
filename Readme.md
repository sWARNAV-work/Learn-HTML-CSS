It seems that I've hit a road block and have to learn HTML and CSS properly before trying to set up a frontend. I've started a Course from Kevin Powell at courses.thecascade.dev . 

### September 26<sup>th</sup>, 2026
- The Three main Languages that make up the web are: HTML, CSS and  JavaScript. Have to learn it in the future.
- The instructor wants us to create a simple website based on Bouldering, which is just rock climbing without any harness. 
- <span class="rh">Use Heading Levels to denote structure, not visually differentiate them. Those h1 h2 h3 things. </span>
- Now making the web page, following the design 1.
- The 'Homepage' 's skeleton HTML has been created. 
- HTML is a <span class="gh">semantic</span> language. 
- The important Sections:- *header , main , section , footer*.
- Some people can not see just as we see. Ex: Handicapped People. This helps them to use the webpages by giving them info of what exactly is. 
- **Header** is what it seems like, It usually serves as the title, company logo, etc etc. 
- **Main** is the section where most of the details are there. **Section** is the different sections within the **Main**.
- **Footer** is, well, The footer. 
- Two tags to help identify text, *strong* and *em*(emphasis). They are **bold** and **italic** respectively.
- Block vs Inline elements. One stacks on top of another and the other is, well, inline.
- **Images** have two attributes, $src$ and $alt$ where *src* stands for Source, and *alt* stands for alternate text.
- Added the images, and created a blank css file. 
- Add the css file to the `<head>` in `index.html` using `<link href="css-source rel="stylesheet">`. `rel` denotes the relationship with the file that is loaded. 
- In CSS we write rules. 
- The styling rules that we create are made up of a few different pieces:- 
  ![[Pasted image 20260926224404.png|250]]
- WWaaww! hex colors go from 0-9 and a-f! Dumb me never thought to check the ranges. In `#5a3b9e` the first two denote  red, then green, then blue. `ff` means full and `00` means zero color, i.e. black. 
- Changed the colors of the different headings and footer in CSS. Cool. 
- Font can be changed using `font-family: Arial, serif;` where Arial is the goto font, if the user doesn't have it then it falls back to serif.
- The browser already has a $UserAgentStyleSheet$ that provides a basic style, that is why the text in HTML work without any CSS. 
- You can also use `: inherit;` to inherit a property.

### September 27<sup>th</sup>, 2026
- Whoa! You should never set the `font-size` to `pixels` in the CSS. It sets the font to that specific size on each and every computer and disregards the custom font sizes that the user might have set up. 
- Instead use `rem`, which resorts to using a scale value of what our html is using. 1 rem mean it's same. 2 is double that.
- `line-height` should always be used as an unitless unit. `margin-block` is used to determine the space above and below a specific type of block.
- CSS can be inlined, but don't use it. Can be used like href using `style=""`. 
- Can also be used in the `head` of an HTML file like `<style></style>`. 
- The Dev Tools inside the browser are pretty handy, they can be used to Debug CSS quite effectively. When you can't find out why something is not working, it is wiser to check the DevTools. 
- Everything in CSS is a box. Thus the next part of CSS, the **Box** Model. ![[Pasted image 20260927121327.png|875]]
- Use logical instead of physical property in CSS whenever possible, i.e., use `inline-size` instead of `width`.
- Similarly, use `block-size` instead of `height`.
- `padding-block` to change top & bottom, `padding-inline` to change left & right.
- `Margins` adds empty space without bg color. `Padding` adds empty space along with the bg color.
- If you add `padding` to any part, the padding starts from outside the element. Suppose you have to set a specific `inline-size`, the border or padding distorts the sizes. To keep them inside the box, there is something called as CSS reset, which is basically a `* {box-sizing: border-box;}` which applies a global sizing method. 
- The Box Model: 
   ![[Pasted image 20260927143538.png|200]]
- Completed the Version 1 of the website and <span class="rh">committed</span> changes.
- D'accord d'abord to Version 2.

### September 28<sup>th</sup>, 2026
- `<div>` and `<span>` are not semantic elements. They are used to organize styling. 
- `<div>` is block level element, whilst `<span>` is an inline element.
- A `<span>` is like a `<strong>` or an `<em>`, without any styling. 
- **Pseudo classes** can be used in CSS, like `a:visited`, that changes things after the link has been visited. 
- Adding images to a `<div>`, there are various new CSS functions to learn. 
- There is something called **Descendent selectors**, so suppose you have to choose a style for the `<strong>` tag inside a CSS class. Then these are useful. ![[Pasted image 20260928191346.png|125]]
- **Specifity** deals with how powerful a selector is. (Hierarchy of which selector will be chosen for styling.). There's a website to check the specificity, https://polypane.app/css-specificity-calculator/. 
- Again, if you can't find something due to this $Specificity$, use the Developer Mode.
- Next on the list is styling lists. yeah? Yeah? Give me Laugh!
- ![[Pasted image 20260928211529.png]]
- To change the color of the bullets only, we have to use **Pseudo Elements**. They are different from pseudo classes cause they are predefined. And a descendent to `<ul>` tag only, otherwise it would be applied to `<ol>` as well. ![[Pasted image 20260928212051.png|125]]
- An emoji or icon can also be used using the `content: 'emoji'` property, in the same way icons or pictures could also be used. 

### September 29<sup>th</sup>, 2026
- There's a new container query in CSS, but that is a class `.container {}` that is commonly used in the wild, to do the same that we will do in the class `.wrapper {}`. 
- To put the content into a fixed size inline, we use `max-inline-size: `, not just inline-size, cause then the webpage will clip when viewing on smaller screens. 
- To center the content on bigger screens, we use `margin-inline: auto;`.
- To format images, use `img {}`, and put `display: block` to use them as block element and not inline element, and use `max-inline-size` here as well to format them for smaller screens, and show the user the full picture no matter what the screen size. 
- There are two boxing options, one is a $**Flexbox**$ and the other is the $**Grid**$ . 
- First we talk about **Grid**, it creates a grid for the children to live in. 
  ![[Pasted image 20260929185959.png]]
- The `grid-template-columns` define how the grid is arranged, as well as how much size they take up. `1fr` stands for 1 fraction of the screen. 
- `gap` denotes the gap between the different items. 
- Setting up the `<nav>` bar now, you should use a label on it called as `aria-label="primary navigation"`, that tells the screen readers what this is.
- The **Flexbox** being the other property, you can use: 
  ![[Pasted image 20260930015245.png|500]]

### September 30<sup>th</sup>, 2026
- There's this something called @ rule, which are CSS functions. It is used in making that RGB animation for the bg of some buttons. 
- <span class="rh">Committing</span>  changes.
- Then there's `@media` query, which has a lot of styles, but we need the `width` style, to prevent clipping of the larger texts when using on a small display. 
- Removed the written link to go from one page to the other. 
- Fixed the photos inside the grid to be left aligned using `margin-inline: auto;`
- Used `@media` to resize the headings and the grids to be a formatted on a mobile-first basis. 
- Final <span class="rh">Commit.</span>
- It came to my knowledge that it is not wise to write such simple commit messages as "Final Commit". The last one should clearly denote what the app does, and in order to rectify my mistakes, I will make another commit. 
- 