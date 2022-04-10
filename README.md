# Frontend Mentor - Stats preview card component

![Design preview for the Stats preview card component coding challenge](./design/desktop-preview.jpg)

# Thoughts and Process

This was pretty fun to make. The biggest thing that I wanted to challenege myself on were media queries. To make the project work, I had to change the media queries to something that wasn't on the style guide. It all worked out in the end. 

Something that that I worked on was using child and sibling seletors. The first time I tried challeng, I created a main wrapper with all the children elements having class names.

```html
<div class="stats-wrapper">
  <div class="stats-body">
    <h1 class="stats-header">...</h1>
  </div>
</div>
```

This is pretty specific, but it felt like there were way too many class names. It felt like child ```>``` and sibling ```+``` selectors would be a better fit. 

```html
<div class="stats-wrapper">
  <div class="stats-body">
    <h1>...</h1>
    <p>...</p>
  </div>
</div>
```

So now my CSS look would like:

```css
.stats-body > h2 {
  margin-bottom: 1em;
}
```

Lastly, this was the first time I used CSS varibles. It made it real easy to use the colors that were outlined in the style guide. Even though they were helpful, the way the varibales have to be called looks really, really ugly. 

```css
.stats-body span {
  color: var(--soft-violet);
}
```

In the end, I think that I got pretty close to the design. I really want to redo this project with Tailwind, and maybe find a way to include Webpack in it. Yea, Webpack. 