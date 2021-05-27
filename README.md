# Eleventy Sane Starter

this project is a starting point for building customisable websites using [Eleventy](https://www.11ty.dev) and [Sanity.io](https://sanity.io).

## Folder structure

* **src**
  _here is where all your custom code lives_

  * **components**
    _Shared ui components go here (eg. navigation, footer, buttons), authored in liquid. If you want to use other templating languages, you have to activate those under `` inside `.eleventy.js`, located in the root folder)_
  
  * **data**
    _Here you can write your queries for retrieving data from sanity_

  * **layouts**
    _Global layouts go here (eg. base layout)_


  * **pages**
    _There are two main types of pages: modular pages (only using portable text inside sanity + SEO/meta info) and custom pages (which always consist of an overview page and subpages. Custom Pages have dedicated fields inside sanity to streamline the authoring process (by not having to manually configure the same fields over again for each new entry)._

    _`src.11tydata.js` is used to configure shared data for all pages (eg. permalink constructor)._

  * **styles**
    _The folder structure inside `styles` is setup to author your styles following the [CUBE.css](https://www.cube.fyi) methology by Andy Bell._

  * **utils**
    _Inside utils you can write filters and shortcodes, which can be used inside your liquid templates. This folder can also accomodate any other handy javascript functions._