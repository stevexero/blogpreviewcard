# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

For this project, my focus will be on font sizes and accessibility. Many users may view sites at different zoom percentages within their browsers, causing fixed font sizes to behave in an unintended manner.

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page
- View a cohesive design regardless of font size.

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it.

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

### Links

- Solution URL: [Frontend Mentor Solution](https://your-solution-url.com)
- Live Site URL: [Blog Preview Card](https://your-live-site-url.com)

## My process

- Reviewed design files for spacing, sizes, colors, etc.
- Set up project folder and files
- Initialized git and GitHub repo
- index.html: Wrapped content in semantic tags
- styles.css: Import fonts, set up reset and root variables
- Set class names and implement base styling
- Refactor for semantic, accessibility, and BEM compliance
- Refactor font sizes to relative units
- Refactor margins and paddings to relative units

### Built with

- Semantic HTML5 markup
- CSS custom properties
- BEM
- Flexbox
- Mobile-first workflow

### What I learned

- The 'time' tag along with the datetime attribute.

> - The <time> tag defines a specific time (or datetime).
> - The datetime attribute of this element is used translate the time into a
>   machine-readable format so that browsers can offer to add date reminders through
>   the user's calendar, and search engines can produce smarter search results.[^1]

```html
<time datetime="2023-12-21">Published 21 Dec 2023</time>
```

- I learned that there is a difference between regular (400) and medium (500) font weights. I always thought they were the same.

- I learned how to implement tooltips. When a user hovers over a link, more information about that link will appear.

```html
<a
  href="#"
  target="_blank"
  rel="noreferrer noopener"
  title="Read more about HTML & CSS foundations"
  >HTML & CSS foundations</a
>
```

- I Learned about figure and figcaption and why we would use them. In my case, it was to group the profile image and the author's name, making it clear that the two are connected with eachother.

> The <figure> HTML element represents self-contained content, potentially with an
> optional caption, which is specified using the <figcaption> element. The figure,
> its caption, and its contents are referenced as a single unit[^2].

> The <figcaption> HTML element represents a caption or legend describing the restof the
> contents of its parent <figure> element, providing the <figure> an accessible description[^3].

- Before figure and figcaption

```html
<footer class="card__footer">
  <a
    href="#"
    target="_blank"
    rel="noreferrer noopener"
    title="Read more articles by Greg Hooper"
  >
    <img src="/assets/images/image-avatar.webp" alt="Headshot of Greg" />
    <p>Greg Hooper</p>
  </a>
</footer>
```

After figure and figcaption

```html
<footer class="card__footer">
  <a
    href="#"
    target="_blank"
    rel="noreferrer noopener"
    title="Read more articles by Greg Hooper"
  >
    <figure>
      <img
        src="/assets/images/image-avatar.webp"
        alt="Headshot of Greg Hooper"
      />
      <figcaption>Greg Hooper</figcaption>
    </figure>
  </a>
</footer>
```

[^1]: Source: [W3Schools.com](https://www.w3schools.com/tags/tag_time.asp)
[^2]: Source: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figure)
[^3]: Source: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/figcaption)

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
