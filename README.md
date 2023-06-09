# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshots

![](./design/Solution-Web.png)
![](./design/Solution-Mobile.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I started with the html and tried to add the sections and classes I would need to use for styling the layout.
Next I worked to get the sections arranged properly using flex
After the placement of the content was correct I started making the specific font sizes and spacing match the design.
Then, I added the hover states for the active elements, including the attribution as a bonus.
Finally I worked on the mobile view, adding a media query to switch the background image and spacing and font-sizes to match the design.
I think it was easier getting the flex components working in the web view before doing the mobile.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Ionicons for the social media icons - which don't exactly match the design but are close enough.

### What I learned

The trickiest part was how images are handled inside a flexbox container. They resize and don't force the other containers to wrap around them without manipulating their min and max sizes.

After some searching I found this to ultimately work best. Along with setting the min-width on the image itself to 50% of the view width to make the wrap happen at a reasonable point.

```css
main img {
  max-height: 100%;
  min-width: 100%;
  object-fit: cover;
  vertical-align: middle;
}
```

### Useful resources

- [Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - I find myself coming back to this page frequently when using flexbox. This site has fantastic resources!
