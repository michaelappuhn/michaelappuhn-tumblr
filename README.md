# blog.michaelappuhn.com tumblr theme

Tumblr template using SASS, Compass, Gulp, and Bower.

## Hi.
I'm taking a weird-looking Game of Thrones themed theme (with an extremely nice production pipeline), merging it with a much nicer starter theme. 

I'll try to save that as a branch, if I remember, for someone else to use, since this is kind of a pain in the ass.


-----

# From the Game of Thrones theme:

## INSTALLATION
### Global Assets
I assume you have installed node & npm (node package manager):

+ https://www.ruby-lang.org/
+ http://nodejs.org/
+ https://www.npmjs.com/

### Necessary packages
```bash
 npm install -g bower  # bower required
 gem install compass   # compass required
```
*Note* When installing compass, be sure it's on your global path.  I had to symlink mine.

### Clone, setup, and gulp
```bash
 git clone https://github.com/shadesoflight/tumblr-template-sass
 cd tumblr-template-sass
 npm install
 bower install
 gulp styles
 gulp scripts
 gulp html --clipboard
```

Gulp will build the theme and put it on your clipboard to paste into your blog

*note, if the HTML task does not start, please restart the process*

All assets are compiled into the build directory in the root of the cloned repository.

A concatenated dist/theme.tumblr file is created, which contains the code to paste into your theme editor.  
To have this file copied onto your clipboard automatically, use `gulp --clipboard` 


------


From the Tumblr Boilerplate theme
------
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/davesantos/tumblr-boilerplate/blob/master/LICENSE.md)

> A fully functional bare-bones Tumblr theme that works out of the box. Style it to your needs. The goal of the project was to remove uncessary code easing the development process.

### Installation

**Bower**

```sh
bower install tumblr-boilerplate
```

**Git**

```sh
git clone https://github.com/davesantos/tumblr-boilerplate.git
```

**Download**

- [Source](https://raw.githubusercontent.com/davesantos/tumblr-boilerplate/master/tumblr.html)
- [Zip](https://github.com/davesantos/tumblr-boilerplate/archive/master.zip)

### Getting Started

1. Choose an [installation](#installation) method.
2. Modify `tumblr.html` with your favorite code editor.
3. Publish it by going to https://www.tumblr.com/customize
4. Click *Edit HTML* on the left column.
5. Copy & paste your customized code then click *Save*.


### Features

* HTML5 tags
* [Normalize.css](https://necolas.github.io/normalize.css/) from [cdnjs](https://cdnjs.com/)
* Supports all [post](https://www.tumblr.com/docs/en/custom_themes#posts) types
* Theme options from [global appeareance](https://www.tumblr.com/docs/en/custom_themes#global_appearance)
* [Localization](https://www.tumblr.com/docs/en/custom_themes#localization) strings

__Theme does not support__

* Comment System ([Disqus](https://disqus.com))
* [Group Blogs](https://www.tumblr.com/docs/en/custom_themes#group-blogs)
* [Notes](https://www.tumblr.com/docs/en/custom_themes#notes)
* [Srcset Attribute](https://caniuse.com/#search=srcset)

(Intentionally not included to remain flexible in the various uses for a theme.)

### Caveats

Tumblr will auto-inject code (such as [Open Graph Protocol](http://ogp.me), [Twitter Cards](https://dev.twitter.com/cards/overview) & javascript) into the final result for your page. This is out of the theme developers' control. Running it through a HTML Validator or Page Speed may spit out warnings & errors.

(Tumblr injects `<!DOCTYPE html>`, twice!)

### Optional Snippets

[Open Graph Protocol](http://ogp.me)<br>
If you choose **not** to include this in your `<head>`, Tumblr will auto-generate it against your will! _Isn't that great!?_

```
<head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# blog: http://ogp.me/ns/blog#">
```
And this:

```
  <meta property="og:site_name" content="{Title}">
  <meta property="og:url" content="{BlogURL}">
  <meta property="og:image" content="{PortraitURL-128}">
  <meta property="og:type" content="tumblr-feed:tumblelog">
```

### Resources
* [Custom Theme Documentation](https://www.tumblr.com/docs/en/custom_themes)
* [tumblr.com/developers](https://www.tumblr.com/developers)
* [Tumblr Developer Blog](http://developers.tumblr.com)
* [HTML5 Boilerplate](https://html5boilerplate.com)
