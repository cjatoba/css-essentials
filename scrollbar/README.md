# Scrollbar tips

## Remove scrollbar style in Chrome, Safari, Internet Explorer, Edge and Firefox but keep functionality
```css
/* Chrome, Safari and Opera */
::-webkit-scrollbar {
    display: none;
}
-ms-overflow-style: none; /* Internet Explorer and Edge */
scrollbar-width: none; /* Firefox */
```

Sources:

https://www.w3schools.com/howto/howto_css_hide_scrollbars.asp
