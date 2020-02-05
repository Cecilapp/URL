# cecil.link

Static URL Shortener powered by [Cecil](https://cecil.app).

## Usage

### Manually

1. Clone the repository
2. Download [Cecil](https://cecil.app/download/)
3. Add file in `content/` directory  
   ie: `ggl.md`  
   ```yaml
   ---
   redirect: https://www.google.com/search?q=cecil+static
   ---
   ```
4. Build the static website: `php cecil.phar build`
5. Deploy `_site` directory on your Web server

### With Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Cecilapp/cecil.link&stack=cms)
