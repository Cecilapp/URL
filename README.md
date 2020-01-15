# cecil.link

Static URL Shortener powered by [Cecil](https://cecil.app).

## Usage

1. Clone the repository

2. Install [Cecil](https://cecil.app/download/)

3. Add one or more URL at the end of [`config.yml`](/config.yml):
   ```
   slug:
     redirect: url
   ```
   
4. Build the website: `php cecil.phar build`

5. Deploy `_site` directory on your Web server

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Cecilapp/cecil.link)
