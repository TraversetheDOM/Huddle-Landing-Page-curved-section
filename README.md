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

## Overview

### The challenge

The users will be able to:

- View the optimal layout for the site depending on their device's screen size.
- The hover states will be seen fro all interective elements on the page.

### Screenshot

![Desktop View](design/Large-Laptops.jpeg)
_A screen shot showing the desktop view_

![Small Laptop View](design/Small-Laptops.jpeg)
_A screen shot showing the view on a small laptop_

![Tablet Sized View](design/Tablet.jpeg)
_A view of the landing page on a tablet_

![A large phone View](design/Large-Phones.jpeg)
_A view of the landing page on a larger sized phone_

![Medium sized view](design/Medium-Phones.jpeg)
_A view of the landing page on a medium sized phone_

![Small sized phone](design/Small-Phones.jpeg)
_The landing page's view on a small phone_

### Links

- Solution URL: [Add solution URL here](https://github.com/salutDami/Huddle-Landing-Page-curved-section)
- Live Site URL: [Add live site URL here](https://salutdami.github.io/Huddle-Landing-Page-curved-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Desktop-first workflow

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Worked alot with flexbox to carry out this project so I was able to learnn how to use some of the properties of flexbox on the flex container and also on the flex items as well.

To see how you can add code snippets, see below:

```html
<div class="container flow_container">
  <figure class="flow_image_holder">
    <img
      src="images/illustration-flowing-conversation.svg"
      alt="a flow illustration image"
      class="flow_image"
    />
  </figure>

  <div class="flow_text_box">
    <h2 class="secondary_heading">Flowing Conversations</h2>
    <p class="secondary_text">
      You wouldn't paginate a conversation in real life, so why do it online?
      Our threads have just-in-time loading for a more natural flow.
    </p>
  </div>
</div>
```

```css
.flow_container {
  display: flex;
  align-items: center;
}

.flow_text_box {
  flex: 0.5;
}

.flow_image {
  max-width: 80%;
}

.flow_text_box > .secondary_heading {
  font-family: var(--ff-Poppins);
  font-weight: var(--fw-700);
  font-size: var(--fs-9);
  color: var(--very-dark-cyan);
  line-height: 1.3;
  margin-bottom: 30px;
}

.flow_text_box > .secondary_text {
  font-family: var(--ff-OpenSans);
  font-weight: var(--fw-400);
  color: var(--very-dark-cyan);
  font-size: var(--fs-5);
  line-height: 1.7;
}

.flow_image_holder {
  flex: 0.5;
  display: flex;
  justify-content: center;
}
```

I also learnt how to use the background image properties to add the curved section to the page as this was actually the toughest part of the project. I added property to the svg which was provided in the file as you can see below;

```css
  preserveAspectRatio="none"
```

```html
<svg
  preserveAspectRatio="none"
  width="375"
  height="101"
  xmlns="http://www.w3.org/2000/svg"
  xmlns:xlink="http://www.w3.org/1999/xlink"
>
  <defs><path id="a" d="M0 0h375v112H0z" /></defs>
  <g fill="none" fill-rule="evenodd">
    <mask id="b" fill="#fff"><use xlink:href="#a" /></mask>
    <g mask="url(#b)" fill="#F6FBFF">
      <path
        d="M-126.345-502.65C14.982-645 139.39-680.588 246.88-609.414c161.235 106.762 291.228 92.307 408.49 0 78.175-61.537 78.175 146.947 0 625.453-127.86 101.604-237.07 122.013-327.628 61.226-135.838-91.181-342.275-91.181-450.675 57.166-72.266 98.899-73.403-113.462-3.41-637.083z"
      />
    </g>
  </g>
</svg>
```

### Continued development

I would surely keep learning and improving on my use of flexbox to make layouts and even more complex one as well. I would also need to get more comfortable with makimg the layouts much better with the use of media queries.

### Useful resources

- [Stackoverflow](https://stackoverflow.com/questions/71104530/google-lighthouse-and-svgs-with-preserveaspectratio-none) - Stackoverflow are a serious life saver for many developers out there and this resources came in handy when working with the curved sections.
- [w3schools](https://w3schools.com) - This webiste really helped when usig flexbox to structure the layout of the landing page.
- [MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox) - This site alos helped as well when I was working with flexbox and I highly recommend it as well.

## Author

- Twitter - [@\_salutDami](https://www.twitter.com/_salutDami)
- Linkedin- [Ikuomola Stephen](https://www.linkedin.com/in/ikuomola-stephen/)
- Frontend Mentor - [@salutDami](https://www.frontendmentor.io/profile/salutDami)
