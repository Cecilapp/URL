# cecil.link

_cecil.link_ is an URL manager (and shortener) powered by [Cecil](https://cecil.app), a static site generator.

## How does it work?

_cecil.link_ is file based, so it nead a file to handle the redirection from the `slug` to the target URL.

So you just have to create this file then _cecil.link_ does the rest of the job.

It create:
1. an HTML file, for each URL, that includes the [HTML redirect](https://developer.mozilla.org/docs/Web/HTTP/Redirections)
2. a [Netlify Redirects](https://docs.netlify.com/routing/redirects/#syntax-for-the-redirects-file) file
3. an Apache .htaccess file

## Usage

### Create an URL

To create a new URL just create a Markdown file in the `content/` directory, with a `redirect` variable stored in the front matter.

#### Example

File name: `ggl.md`

File content:
```yaml
---
redirect: https://www.google.com/search?q=cecil+static
---
```

Demo: https://cecil.link/ggl

### Build and deploy

1. Clone the repository
2. Download [Cecil](https://cecil.app/download/)
4. Build the static website: `php cecil.phar build`
5. Deploy the `_site` directory on your Web server

#### With Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Cecilapp/cecil.link&stack=cms)
