<div id="top"></div>

<!-- PROJECT SHIELDS -->
<!--
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
-->

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <!-- <a href="https://github.com/anandang76/stringting_code_update">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a> -->
  <h3 align="center">StringTing Website Changes</h3>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#assets">Assets</a>
    </li>
    <li><a href="#Layouts">Layouts</a></li>
    <li><a href="#Section">Section</a></li>
    <li><a href="#Snippets">Snippets</a></li>
    <li><a href="#Templates">Templates</a></li>
    <li><a href="#CssUpdate">CssUpdate</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## Assets

Added Grold Rounded Font to implus theme

### Layouts

Added stamped.io, klaviyo, product slider script in layout theme.liquid file

Added Stampled.io 
```html
<!-- Stamped - Begin Script-->
<script async type="text/javascript" data-api-key="" id="stamped-script-widget" src="https://cdn-stamped-io.azureedge.net/files/widget.min.js"></script>
<!-- Stamped - End Script -->
```
Added Slick Carosel
```html
<script src="https://code.jquery.com/jquery-1.11.0.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.js" integrity="sha512-XtmMtDEcNz2j7ekrtHvOVR4iwwaD6o/FUJe6+Zq+HgcCsk3kj4uSQQR8weQ2QVj1o0Pk6PwYLohm206ZzNfubg==" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css" integrity="sha512-17EgCFERpgZKcm0j0fEq1YCJuyAWdz9KUtv1EjVuaOz8pDnh/0nZxmU6BBXwaaxqoi9PQXnRWqlcDB027hgv9A==" crossorigin="anonymous" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css" integrity="sha512-yHknP1/AwR+yx26cB1y0cjvQUMvEa2PFzt1c9LlS4pRQ5NOTZFWbhBig+X9G9eYW/8m0/4OXNx8pxJ6z57x0dw==" crossorigin="anonymous" />
```
Added Flickity Slider
```html
<script src=“https://unpkg.com/flickity@2/dist/flickity.pkgd.min.js”></script>
<link rel=“stylesheet” href=“https://unpkg.com/flickity@2/dist/flickity.min.css”>
```
Added Klaviyo Form for footer
```html
<script async type="text/javascript" src="https://static.klaviyo.com/onsite/js/klaviyo.js?company_id=SF9adq"></script>
```
Added Product Slider script
```html 
  <script>
  $(document).ready(function() {
  $(".flex-grid__item--promo-0, .flex-grid__item--promo-1").click(function(){
   console.log("Redirect to shop");
   window.location.href="/collections/"   
  });
 
 
$('.collection-slider').slick({ // use the main class name of all images here.
  dots: true,
  infinite: true,
  speed: 300,
  slidesToShow: 4,
  slidesToScroll: 1,
  autoplay: false,
  autoplaySpeed: 2000,
  responsive: [
    {
      breakpoint: 1024,
      settings: {
        slidesToShow: 3,
        slidesToScroll: 3,
        infinite: true,
        dots: true
      }
    },
    {
      breakpoint: 600,
      settings: {
        slidesToShow: 2,
        slidesToScroll: 1
      }
    },
    {
      breakpoint: 480,
      settings: {
        slidesToShow: 2,
        slidesToScroll: 2
      }
    }
    // You can unslick at a given breakpoint now by adding:
    // settings: "unslick"
    // instead of a settings object
  ]
});
});
</script>

```


### Section

Added following sections
* custom-clear-pay-later.liquid
* custom-desktop-banner.liquid
* custom-feature-slider.liquid
* custom-flickity.liquid
* custom-how-to-page.liquid
* custom-logos.liquid
* custom-mobile-banner.liquid
* custom-mobile-separator.liquid
* custom-page-our-tings.liquid
* custom-pay-later.liquid
* custom-product-review.liquid
* custom-products-carousel.liquid
* custom-seperator.liquid
* custom-static-testimonial.liquid
* custom-testimonial.liquid

### Snippets

Added following snippets
* custom-flickity-slider.liquid
* custom-mobile-footer.liquid
* footer-custom-html.liquid
* footer-custom-text.liquid


### Templates
Added following Page Template added

* page.custom-how-to.liquid
* page.custom-our-tings.liquid
* page.custom-about.liquid

### CssUpdate
Css update in theme.css.liquid

* Add font 
```css
   @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-SemiLight.eot");
        src: local("Grold Rounded SemiLight"), local("GroldRounded-SemiLight"), url("GroldRounded-SemiLight.eot?#iefix") format("embedded-opentype"), url("GroldRounded-SemiLight.woff2") format("woff2"), url("GroldRounded-SemiLight.woff") format("woff"), url("GroldRounded-SemiLight.ttf") format("truetype"), url("GroldRounded-SemiLight.svg#GroldRounded-SemiLight") format("svg");
        font-weight: 300;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-ExtraBold.eot");
        src: local("Grold Rounded ExtraBold"), local("GroldRounded-ExtraBold"), url("GroldRounded-ExtraBold.eot?#iefix") format("embedded-opentype"), url("GroldRounded-ExtraBold.woff2") format("woff2"), url("GroldRounded-ExtraBold.woff") format("woff"), url("GroldRounded-ExtraBold.ttf") format("truetype"), url("GroldRounded-ExtraBold.svg#GroldRounded-ExtraBold") format("svg");
        font-weight: bold;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-SemiLightItalic.eot");
        src: local("Grold Rounded SemiLight Italic"), local("GroldRounded-SemiLightItalic"), url("GroldRounded-SemiLightItalic.eot?#iefix") format("embedded-opentype"), url("GroldRounded-SemiLightItalic.woff2") format("woff2"), url("GroldRounded-SemiLightItalic.woff") format("woff"), url("GroldRounded-SemiLightItalic.ttf") format("truetype"), url("GroldRounded-SemiLightItalic.svg#GroldRounded-SemiLightItalic")format("svg");
        font-weight: 300;
        font-style: italic;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-MediumItalic.eot");
        src: local("Grold Rounded Medium Italic"), local("GroldRounded-MediumItalic"), url("GroldRounded-MediumItalic.eot?#iefix") format("embedded-opentype"), url("GroldRounded-MediumItalic.woff2") format("woff2"), url("GroldRounded-MediumItalic.woff") format("woff"), url("GroldRounded-MediumItalic.ttf") format("truetype"), url("GroldRounded-MediumItalic.svg#GroldRounded-MediumItalic") format("svg");
        font-weight: 500;
        font-style: italic;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-Medium.eot");
        src: local("Grold Rounded Medium"), local("GroldRounded-Medium"), url("GroldRounded-Medium.eot?#iefix") format("embedded-opentype"), url("GroldRounded-Medium.woff2") format("woff2"), url("GroldRounded-Medium.woff") format("woff"), url("GroldRounded-Medium.ttf") format("truetype"), url("GroldRounded-Medium.svg#GroldRounded-Medium") format("svg");
        font-weight: 500;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-Bold.eot");
        src: local("Grold Rounded Bold"), local("GroldRounded-Bold"), url("GroldRounded-Bold.eot?#iefix") format("embedded-opentype"), url("GroldRounded-Bold.woff2") format("woff2"), url("GroldRounded-Bold.woff") format("woff"), url("GroldRounded-Bold.ttf") format("truetype"), url("GroldRounded-Bold.svg#GroldRounded-Bold") format("svg");
        font-weight: bold;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-BlackItalic.eot");
        src: local("Grold Rounded Black Italic"), local("GroldRounded-BlackItalic"), url("GroldRounded-BlackItalic.eot?#iefix") format("embedded-opentype"), url("GroldRounded-BlackItalic.woff2") format("woff2"), url("GroldRounded-BlackItalic.woff") format("woff"), url("GroldRounded-BlackItalic.ttf") format("truetype"), url("GroldRounded-BlackItalic.svg#GroldRounded-BlackItalic") format("svg");
        font-weight: 900;
        font-style: italic;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-Black.eot");
        src: local("Grold Rounded Black"), local("GroldRounded-Black"), url("GroldRounded-Black.eot?#iefix") format("embedded-opentype"), url("GroldRounded-Black.woff2") format("woff2"), url("GroldRounded-Black.woff") format("woff"), url("GroldRounded-Black.ttf") format("truetype"), url("GroldRounded-Black.svg#GroldRounded-Black") format("svg");
        font-weight: 900;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-Regular.eot");
        src: local("Grold Rounded Regular"), local("GroldRounded-Regular"), url("GroldRounded-Regular.eot?#iefix") format("embedded-opentype"), url("GroldRounded-Regular.woff2") format("woff2"), url("GroldRounded-Regular.woff") format("woff"), url("GroldRounded-Regular.ttf") format("truetype"), url("GroldRounded-Regular.svg#GroldRounded-Regular") format("svg");
        font-weight: normal;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-Light.eot");
        src: local("Grold Rounded Light"), local("GroldRounded-Light"), url("GroldRounded-Light.eot?#iefix") format("embedded-opentype"), url("GroldRounded-Light.woff2") format("woff2"), url("GroldRounded-Light.woff") format("woff"), url("GroldRounded-Light.ttf") format("truetype"), url("GroldRounded-Light.svg#GroldRounded-Light") format("svg");
        font-weight: 300;
        font-style: normal;
        font-display: swap
    }

    @font-face {
        font-family: "Grold Rounded";
        src: url("GroldRounded-Italic.eot");
        src: local("Grold Rounded Italic"), local("GroldRounded-Italic"), url("GroldRounded-Italic.eot?#iefix") format("embedded-opentype"), url("GroldRounded-Italic.woff2") format("woff2"), url("GroldRounded-Italic.woff") format("woff"), url("GroldRounded-Italic.ttf") format("truetype"), url("GroldRounded-Italic.svg#GroldRounded-Italic") format("svg");
        font-weight: normal;
        font-style: italic;
        font-display: swap
    }

    html, body{
        font-family: "Grold Rounded", sans-serif !important;
    }

```


* Update other styles


```css

    /***
    *  Footer css
    *
    ***/

    .footer-logo {
        text-align: center;
    }

    .footer-top-img {
        text-align: center;
    }

    img.footer-group-img {
        width: 47%;
        text-align: center;
    }

    .footer-socials>ul {
        list-style-type: none;
    }

    li.single-footer-social-item {
        display: inline-block;
        padding: 5px;
    }

    li.single-footer-social-item>a {
        border: 1px solid black;
        /*     padding: 17px 11px 7px 12px; */
        border-radius: 50%;
    }

    ul.no-bullets>li>a {
        font-weight: 400;
        font-size: 17px;
    }

    .site-footer__linklist>li {
        margin-bottom: -3px;
    }


    /***
    *  Footer css
    *
    ***/


    /***
    *  Home page css
    *
    ***/

    .slick-next,
    .slick-prev {
        z-index: 10 !important;
    }

    .type-advanced .promo-grid__content:not(.promo-grid__content--boxed):not(.promo-grid__content--sale),
    .type-simple .promo-grid__content:not(.promo-grid__content--boxed):not(.promo-grid__content--sale) {
        color: #fff;
        color: var(--colorHeroText);
        width: 100%;
        background: #000;
    }

    .custom-separator {
        border-top: 2px solid #d20a50;
        margin: 15px 0px;
    }

    h2.section-header__title {
        font-size: 23px !important;
    }

    .logo-bar--template--15612524134622__164403944613f830fe {
        opacity: 1.0;
        margin-top: -36px;
    }

    .logo-bar--template--15612524134622__164386551818fccd84 {
        opacity: 1.0;
        margin-top: 35px;
    }

    div#shopify-section-template--15612524134622__164398240992d2a2eb {
        margin-top: 75px;
    }

    form#localization_form {
        width: 50px;
    }

    .fa-star,
    .fa-star-checked,
    .fa-star-half-o,
    .fa-star-o,
    .stamped-fa-star,
    .stamped-fa-star-checked,
    .stamped-fa-star-half-o,
    .stamped-fa-star-o {
        color: #000 !important;
        padding: 0;
    }

    @media screen and (max-width:920px) {
        img.footer-group-img {
            width: 80%;
            text-align: center;
        }
    }

    @media screen and (max-width:600px) {
        .logo-bar.logo-bar--template--15612524134622__164403944613f830fe {
            margin-top: -14px;
        }
    }

    .slick-dotted.slick-slider {
        margin-bottom: 0 !important;
    }


    /**
    ** Header Css
    ** 
    ***/

    div#fsb_container {
        display: none !important;
        visibility: hidden !important;
    }

    @media screen and (max-width:600px) {
        .site-nav__icons {
            white-space: nowrap;
            margin-top: 5px;
        }
    }

    @media screen and (max-width:412px) {
        .site-header__logo a {
            width: 200px;
            font-size: 27px;
        }
    }

    .custom-product-carosuel-header>h2 {
        font-weight: 700;
        font-family: 'Grold Rounded', serif;
        font-size: 40px;
    }

    @media screen and (max-width:480px) {
        .custom-product-carosuel-header>h2 {
            font-weight: 700;
            font-family: 'Grold Rounded', serif;
            font-size: 28px;
        }
    }

    .rte--block.rte--strong {
        margin: 0 !important;
    }

    @media screen and (max-width:768px) {
        .custom-mobile-separator {
            border-top: 2px solid #d20a50 !important;
            margin: 15px 0px;
        }
    }

    div#StickyHeaderWrap {
        height: auto !important;
    }

    @media only screen and (max-width: 767px) {
        .flex-grid.flex-grid--gutters.flex-grid--template--15612524134622__promo-grid {
            margin-right: 0;
            padding-right: 0 !important;
        }
        .flex-grid__item.type-advanced {
            margin-left: 0;
            padding-left: 0 !important;
        }
    }

    .promo-grid__content {
        cursor: pointer;
    }

    .flex-grid__item--promo-0,
    .flex-grid__item--promo-1 {
        cursor: pointer;
    }

```

<p align="right">(<a href="#top">back to top</a>)</p>
