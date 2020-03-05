# Natours Project

## 6. Building The Header - Part 1

* Write HTML for Header

``` html
<header class="header">Some Text...</header>
```

* Create universal Reset

``` css

* {

    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

* Add font styling to body tag

``` css
body {
    font-family: "Lato", sans-serif;
    font-weight: 400;
    font-size: 16px;
    line-height: 1.7;
    color: #777;
    padding: 30px;
}
```

* Add .header class styling

``` css
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

## 7. Building The Header - Part 2

* Add the main heading and wrap it into 2 spans inside an H1 element. H1 is the most important header on the website so we ensure it contains the main focus of the site.

``` html
<div class="text-box">
    <h1 class="heading-primary">
        <span class="heading-primary-main">Outdoors</span>
        <span class="heading-primary-sub">is where life happens</span>
    </h1>
</div>
```

* We position the text-box, to 50% from top and from the left to the **center** of the page. This targets the edge of the text-box so the content still needs to be adjusted. To do this we translate the the heading-primary, (the content of the text-box) by -50% for both the y and x axis, to move it to where the **center** is located.

``` css
.text-box {
    position: absolute;
    top: 40%;
    left: 50%;
    transform: translate(-50%, -50%);
}
```

* We add simple text styles for the headings.

``` css
.heading-primary {
    color: #fff;
    text-transform: uppercase;
}

.heading-primary-main {
    display: block;
    font-size: 60px;
    font-weight: 400;
    letter-spacing: 35px;
}

.heading-primary-sub {
    display: block;
    font-size: 20px;
    font-weight: 700;
    letter-spacing: 17.4px;
}
```

 - - -
