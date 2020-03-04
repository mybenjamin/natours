# 6. Building The Header - Part 1

## A. Write HTML for Header

```html
<header class="header">Some Text...</header>
```

## B. Create universal Reset

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

## C. Add font styling to body tag

```css
body {
    font-family: "Lato", sans-serif;
    font-weight: 400;
    font-size: 16px;
    line-height: 1.7;
    color: #777;
    padding: 30px;
}
```

## D. Add .header class styling

```css
.header {
    height: 95vh;
    background-image:
        linear-gradient(to right bottom,
            rgba(123, 213, 11, 0.8),
            rgba(40, 180, 131, 0.8)),
        url(../img/hero.jpg);
    background-size: cover;
    background-position: top;

    clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%)
}
```

- - -
- - -
- - -

