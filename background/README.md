# Tips for background

## Set background image and apply opacity without affecting children's elements

```html
<div class="parent">
  <section>Content</section>
</div>
```

```css
.parent {
  width: 100%;
  height: 100vh;

  ::before {
    content: "";
    position: absolute;
    inset: 0;
    /* Remove linear-gradient property if you don't want to apply gradient */
    background-image: linear-gradient(to right, #07080a, transparent 50%),
      linear-gradient(to bottom, transparent 40%, #07080a 70%),
      url("https://imageurl.com");
    background-repeat: no-repeat;
    background-position: top right;
    background-size: 100%;
    z-index: -1;
    opacity: 0.5;
  }
}
```
