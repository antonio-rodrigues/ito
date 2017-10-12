# ITO UNICENTER TNG


This is the official repository for [ITO UNICENTER TNG](http://www.itounicentertng.pt).

The website was built on top of ZURB's Fundation. It has a Gulp-powered build system with these features:

- Handlebars HTML templates with Panini
- Sass compilation and prefixing
- JavaScript module bundling with webpack
- Built-in BrowserSync server
- For production builds:
  - CSS compression
  - JavaScript compression
  - Image compression

## Installation

To use this repo, your computer needs:

- [NodeJS](https://nodejs.org/en/) (0.12 or greater)
- [Git](https://git-scm.com/)

Project also needs the Foundation CLI.

### Installing the CLI

Install the Foundation CLI with this command:

```bash
npm install foundation-cli --global
```

To run in development mode: `cd` to your project folder and to start your project run 

```bash
foundation watch
```

You can adjust `BrowserSync` (auto-refresh) options accessing:
```
http://localhost:3001
```


### Cloning the project

To clone the project run Git on command line:

```bash
git clone https://github.com/antonio-rodrigues/ito.git
```

Then open the folder in your command line, and install the needed dependencies:

```bash
cd ito
npm install
```

Finally, run `npm start` to run Gulp. Your site will be created in a folder called `dist`, viewable at this URL:

```
http://localhost:8000
```

To create compressed, production-ready assets, run `npm run build`.

Note: if you find that icon images are missing, please copy all files from `/etc` folder into `/dist/assets/css/` folder.

### Deploy to cloud

To deplay the website to your server, run: `npm run build`.

Then upload all files inside folder `/dist` to the server (normally, `/public_html` folder).
