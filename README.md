<div align="center">
  <a href="https://github.com/pictura-io/API-description"><img width="100%" src="http://res.cloudinary.com/drcolkwyx/image/upload/v1517770288/Pictura_logo_-_git_jzkhdw.png" alt="Pictura api logo" /></a>
</div>


# Pictura API - Create dynamic meta images [![Gitter](https://badges.gitter.im/Join%20Chat.svg)][gitter]

[gitter]: https://gitter.im/Pictura-API

When URL is shared on Social Media, our API gets Facebook/Linkedin crawlers' request and dynamically creates/modifies an image by either: Taking an image from a page and combining with your template (The Guardian Example) OR Opening a page and taking a screenshot (Bridgestone job ad example).

<div align="center" style="display: inline-block;">
  <a href="https://www.pictura.io/"><img width="35%" src="https://www.pictura.io/assets/pictura-guardian-example-f9a84a06bf0e8c6fc96c18d1b28d1707b1f3eb8cebc2bbdf75209b81ef150058.png" alt="Pictura guardian example" /></a><a href="https://www.pictura.io/"><img width="35%" src="https://www.pictura.io/assets/pictura-bridgestone-example-ba0593e3693fb9ab0b4981138653bea3c09d8d2ac6556c51f900221556901c41.png" alt="Pictura screenshot example" /></a>
</div>

## Features
Keep it light weight on your side and give us all the heavy lifting.

* Stable and scalable amazon AWS (Lambda & S3) infrastructure
* Chromium - Google browser project
* Image delivery through CDN.
* Secure SSL connections.


## Integration (5min)

```html
<meta property="og:image" contet="https://api.pictura.io?url=https://YOUR-PAGE.com"/>
```

### Full Step-by-Step Guide

#### Step 1: Register
First step is to <a href="https://www.pictura.io/users/sign_up">register</a> at Pictura.io platfrom


#### Step 2: Sub/domains setup
Once registered, copy and paste your websites' page to save domain name under setup page. We will use it to identify shared pages. If you have multiple domains, subdomains or nested url where you like to make individual custom setups, then you need to click on 'add more & edit - Advanced' button and setup each one.


#### Step 3: Display selection
Select how you would like your meta images shared on social media to look like. You can choose from 2 options: making a screenshot of your page or combining images from your page with your uploaded template.

#### Step 4: Make it Dynamic & integrate
Once setup of domains/subdomains is made, you then need to replace your existing meta og:image tags with Pictura API and provide dynamic parameters such as given page url. Here is the example for Javascript.


```html
<meta property="og:image" content="https://api.pictura.io?url=${encodeURIComponent(window.location.href)}" />
<meta property="og:image:type" content="image/png" />
<meta property="og:image:width" content="1200" />
<meta property="og:image:height" content="630" />
```

