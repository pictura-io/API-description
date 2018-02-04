<div align="center">
  <a href="https://github.com/pictura-io/API-description"><img width="100%" src="http://res.cloudinary.com/drcolkwyx/image/upload/v1517770288/Pictura_logo_-_git_jzkhdw.png" alt="Pictura api logo" /></a>
</div>


# Pictura API - Create dynamic meta images [![Gitter](https://badges.gitter.im/Join%20Chat.svg)][gitter]

[gitter]: https://gitter.im/Pictura-API

When URL is shared on Social Media, our API
gets a request and dynamically creates an image by either: Taking an image from a page and combining with your template OR Opening a page and taking a screenshot

<div align="center" style="display: inline-block;">
  <a href="https://www.pictura.io/"><img width="40%" src="https://www.pictura.io/assets/pictura-guardian-example-f9a84a06bf0e8c6fc96c18d1b28d1707b1f3eb8cebc2bbdf75209b81ef150058.png" alt="Pictura guardian example" /></a>
<span style="width: 20%;"></span>
  <a href="https://www.pictura.io/"><img width="40%" src="https://www.pictura.io/assets/pictura-bridgestone-example-ba0593e3693fb9ab0b4981138653bea3c09d8d2ac6556c51f900221556901c41.png" alt="Pictura screenshot example" /></a>
</div>

## Features

* Stable and scalable amazon AWS (Lambda & S3) infrastructure
* Chromium (Google browser project)
* Image delivery through CDN.
* Secure SSL connections.


## Integration (5min)

```html
<meta property = "og:image" contet = "https://api.pictura.io?url=https://YOUR-PAGE.com" />
```
