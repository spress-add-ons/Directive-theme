## Directive theme for Spress

Directive is a ported theme to Spress design by [HTML5 UP](http://html5up.net).

[Live demo](http://spress-add-ons.github.io/directive/).

### Featured:

* Responsive design: Support to mobile and tablets.
* Top and bottom menu.
* Social networks link at the footer.
* Sitemap and RSS feed.

### How to install?

#### Download a copy

* Get a copy of the latest [release](https://github.com/spress-add-ons/Directive-theme/releases).
* Uncompress it.
* Go to `Directive-theme` folder
* `spress site:build --server --watch`

#### With Git

* [Fork this repository](https://github.com/spress-add-ons/Directive-theme/fork)
* Clone it: ` https://github.com/YOUR-USER/Directive-theme.git
* Go to `Directive-theme` folder
* `spress site:build --server --watch`

#### Globally

Some way to do it.

Go to your [Spress](http://spress.yosymfony.com/) installation folder i.e  **~/Spress** and add the following depencency to your `composer.json` file 

```json
"require": {
    "spress-add-ons/directive-theme": "1.0.*@dev"
}
```

and then run the following command to install the dependency.

```bash
$ composer update
```

Next create your new site:

```bash
$ spress new:site /your-site-dir directive
$ cd /your-site-dir
$ spress site:build --server --watch
```

### Configuration

#### Menus

Spresso support top and bottom menus. To configure, you can edit
`top_menu` and `bottom_menu` options from the `config.yml`:

```yaml
top_menu:
    - { name: Home, url: / }
    - { name: About, url: /about }

    # To generate a absolute URL using site.url value:
    - { name: Docs, url: /docs, site_url: true}
    
bottom_menu:
    - { name: Your link, url: https://your-url }
```

#### Comments

Comments are powered by [Disqus](disqus.com) and it need your 
**disqus shortname**. To get it, you need create a account at this service.
It's free.

##### Disable comments

By default, Disqus comments are enabled. If you want a post without comments, set
the `comments` variable to `false` at the Front-matter of the post:

```yaml
---
comments: false
---
```

### License 
Free for personal and commercial use under the [CCA 3.0 license](https://creativecommons.org/licenses/by/3.0/)
