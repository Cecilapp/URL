# cecil.link

_cecil.link_ is an URL manager / shortener powered by [Cecil](https://cecil.app), a static site generator.

## Usage

### Create an URL

_cecil.link_ is a file based manager, so to create a new URL, just a create a Markdown file in the `content/` directory, with a `redirect` variable stored in the front matter.

#### Example

File name: `ggl.md`

File content:
```yaml
---
redirect: https://www.google.com/search?q=cecil+static
---
```

Demo: https://cecil.link/ggl

### Installation

1. Clone the repository
2. Download [Cecil](https://cecil.app/download/)
4. Build the static website: `php cecil.phar build`
5. Deploy the `_site` directory on your Web server

#### With Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Cecilapp/cecil.link&stack=cms)
