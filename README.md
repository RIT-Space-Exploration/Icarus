# Mapache for [Ghost](https://github.com/tryghost/ghost/)

[![Ghost version](https://img.shields.io/badge/Ghost-1.x-brightgreen.svg?style=flat-square)](https://ghost.org/)
[![Node version](https://img.shields.io/node/v/uno-zen.svg?style=flat-square)](https://nodejs.org/en/)
[![Donate](https://img.shields.io/badge/donate-paypal-blue.svg?style=flat-square)](https://bit.ly/PayPal-GodoFredoNinja)

> Minimalist Material Design and Elegant theme for [Ghost](https://github.com/tryghost/ghost/)

## Free theme for Ghost

Bases on the GogoFredo Ninja theme

### 😃 To have updated the subject please help me with a small collaboration in [paypal](https://bit.ly/PayPal-GodoFredoNinja). I will thank you enormentene

[![](./documentation/donate.gif)](https://bit.ly/PayPal-GodoFredoNinja)

![](./documentation/mapache-screenshot.png)

## Demo

> Later I will write an article showing the functionality of the theme. For the moment in my page I am using one of my theme [simply](https://github.com/godofredoninja/simply)

You can see a demo in my [blog](http://bit.ly/GodoFredoNinja-Mapache).

## Mapache Support for Web Browsers

Mapache supports the following web [browsers](http://caniuse.com/#search=flexbox)

## Featured

- Support for different [languages](http://themes.ghost.org/docs/i18n#section-how-to-add-any-language) (en - es)
- Responsive layout
- Blog navigation
- Home title Typed style
- Page 404 (Multiple faces emoticons)
- Page subscribe
- Pagination Infinite Scroll
- Cover images for blog, tag and author
- links to followers in social media
- Related Articles (6 articles)
- Template (Video Post Format)
- Teamplate (Image post Format)
- Template (Audio post Format)
- AMP Template (Accelerated Mobile Pages)
- 5 articles featured in the home of the page section sidebar
- 5 articles latest posts in the (author - tag - post) section sidebar
- 10 Tags in the sidebar
- Support for comments (Facebook or Disqus)
- Support for counter comments (Facebook or Disqus)
- Buttons to share the article
- YouTube, Vimeo, kickstarter, dailymotion, vid.me -> Video Responsive
- YouTube Subscribe Button => Video Post Format
- Facebook widget in sidebar
- Twitter widget in sidebar
- Code syntax [Prismjs](http://prismjs.com/index.html) Supported all syntax.

## Ghost settings

- Enable **all** checkboxes on the labs page in your Ghost admin panel.

![](./documentation/img-api.png)

## Mapache settings

### Social Links

Add the Social Links only for the services you want to appear in the header section of your website. Pay attention as enabling too many services will cause menu problems.

### YouTube Subscribe Button

This section enables the YouTube Post format. Add the Channel Name and Channel ID which can be found here [YouTube Advanced Settings](https://www.youtube.com/account_advanced)

— Copy the below script to `Settings -> Code Injection  -> Blog Footer section`

```html
<script>
/*====================================================
  THEME SETTINGS & GLOBAL VARIABLES
====================================================*/

/* 01. Social Media Follow */
var followSocialMedia = {
  'google': 'https://...',
  'youtube': 'https://...',
  'instagram': 'https://...',
  'snapchat': 'https://...',
  'dribbble': 'https://...',
  'github': 'https://...',
  'linkedin':'https://...',
  'spotify':'https://...',
  'codepen':'https://...',
  'behance':'https://...',
  'flickr':'https://...',
  'pinterest':'https://...',
  'telegram':'https://...',
  'discord':'https://...',
  'feed':'https://...',
};

/* 02. Title for home Page */
var homeTitle = '... your title ...';

/* if you want to have the title style typed
ignore homeTitle and add this code */
var homeTitleTyped = ['YOUR TITLE 1', 'YOUR TITLE 2', 'YOUR TITLE 3', 'YOUR TITLE 4'];

/* 03. Home BTN <SUBSCRIBE> */
var homeBtnTitle = 'Name BTN';
var homeBtnURL = 'https://...';

/* 04. Youtube button subscribe for Video Post Format */
var youtubeChannelName = 'YOUR_CHANNEL_NAME';
var youtubeChannelID = 'YOUR_CHANNEL_ID';

/* 05. Disqus Comment Settings */
var disqusShortName = 'YOUR_DISQUS_SHORTCUT_HERE';

/* 06. Facebook Widget Settings */
var fansPageName = 'YOUR_FANS_PAGE_NAME';

/* 07. Twitter Widget Settings */
var twitterUserName = 'YOUR_TWITTER_NAME';
var twitterNumber = 2;
</script>

<!-- Disqus Comments Count-->
<script id="dsq-count-scr" src="//YOUR_DISQUS_SHORTCUT_HERE.disqus.com/count.js" async></script>
```

### Facebook Comments

To use facebook comments, skip the configuration Disqus.

This enables comments and comment counter

— Add the code `Settings -> Code Injection -> Blog Footer`

```html
  <div id="fb-root"></div>
  <script>(function(d, s, id) {
    $('.mapache-facebook').removeClass('u-hide');
    var js, fjs = d.getElementsByTagName(s)[0];
    if (d.getElementById(id)) return;
    js = d.createElement(s); js.id = id;
    js.async=true;
    js.src = 'https://connect.facebook.net/en_US/sdk.js#xfbml=1&version=v2.11';
    fjs.parentNode.insertBefore(js, fjs);
  }(document, 'script', 'facebook-jssdk'));</script>
```

## Publication Language

**Mapache supports:**

- `en` — English default language
- `es` — Español
- `de` — German

![](./documentation/language.png)

if you want to have in another language you just have to copy `locales>en.json` and rename the file then translate to your favorite language:

Just enter the [language/locale tag](https://www.w3schools.com/tags/ref_language_codes.asp) of the files to use (e.g.: `fr.json` for French, `zh.json` for Chinese, `ja.json` for Japanese)

## Change Theme Style

To change the color of the Mapache theme select one of the theme styles below and copy it into the Setting -> Code Injection -> Blog Header

```html
<!-- Theme indigo -->
<link rel="stylesheet" href="/assets/styles/theme-indigo.css"/>
<!-- Theme dark blue -->
<link rel="stylesheet" href="/assets/styles/theme-dark-blue.css"/>
<!-- Theme blue semi dark -->
<link rel="stylesheet" href="/assets/styles/theme-blue-semi-dark.css"/>
<!-- Theme blue -->
<link rel="stylesheet" href="/assets/styles/theme-blue.css"/>
<!-- Theme Grey -->
<link rel="stylesheet" href="/assets/styles/theme-grey.css"/>
<!-- Theme dark cyan -->
<link rel="stylesheet" href="/assets/styles/theme-dark-cyan.css"/>
<!-- Theme purple -->
<link rel="stylesheet" href="/assets/styles/theme-purple.css"/>
<!-- Theme teal -->
<link rel="stylesheet" href="/assets/styles/theme-teal.css"/>
<!-- Theme Green -->
<link rel="stylesheet" href="/assets/styles/theme-green.css"/>

<!-- For theme white add two-color logo 230px * 130px -->

<!--
  ***** 230px *****
  *               *
  ***************** 130px
  *               *
  *****************
-->


<link rel="stylesheet" href="/assets/styles/theme-white.css"/>
```

![](./documentation/img-four.png)

### Add additional content to the sidebar

Add you own custom content into the side bar by editing the `./partials/sidebar.hbs` file.

```html
<!-- Add your content to the bottom -->
<div class="sidebar-items">
  <div class="sidebar-title">...your title...</div>
  ... your content ...
</div>
```

### Warning - Note - Success

Add some more styling options to your articles text with these three styles.

```html
<p class="warning"> ... your text warning ... </p>

<p class="note"> ... your text note ... </p>

<p class="success"> ... your text success ... </p>
```

![](./documentation/note.png)

### PrismJS code syntax

Make your code stand out. WIth the PrismJS code highlighter. PrismJS allows you to select which languge you embeded and performs code highlighting according to the language. Neat!

Take a look at the [Prismjs Supported Language List](http://prismjs.com/#languages-list)

![](./documentation/code.png) to find your coding language.

## Template for (Video - Image - Audio)

**Image** — The Featured image will become large in size.

**Video** — The first video in the article will be large in size. Supports formats

- vimeo
- Dailymotion
- Youtube
- Vid
- kickstarter

**Audio** — The first Audio in the article will be large in size. Supports formats

- Soundcloud
- Mixcloud
- Spotify

> Add video or Audio where convenient. When you change the theme you will not have problems and not have Problem in your AMP Template

![](./documentation/video-format.png)

![](./documentation/video.png)

### Credits

- [Hodor AMP Template](https://github.com/godofredoninja/Hodor-AMP-Template-for-Ghost)
- [Typed](https://github.com/mattboldt/typed.js/)
- [Normalize](https://necolas.github.io/normalize.css/)
- [Jquery.ghostHunter](https://github.com/jamalneufeld/ghostHunter)
- [Prismjs](http://prismjs.com/)
- [theia-sticky-sidebar](https://github.com/WeCodePixels/theia-sticky-sidebar)
- [jquery-lazyload](http://www.appelsiini.net/projects/lazyload)

## Copyright & License

Copyright (c) 2016 @GodoFredoNinja - Released under the [MIT license](LICENSE).
