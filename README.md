## Directive theme for Spress

Directive is a ported theme to Spress design by [HTML5 UP](http://html5up.net).
[Live demo](http://spress-add-ons.github.io/directive/).

### License 
Free for personal and commercial use under the [CCA 3.0 license](http://html5up.net/license)

### Featured:

* Responsive design: Support to mobile and tablets.
* Top and bottom menu.
* Social networks link at the footer.
* Sitemap and RSS feed.

### How to install?

Go to your Spress installation folder and add the following to your `composer.json`
and run `composer update`:

```
"require": {
    "spress-add-ons/directive-theme": "~1.0-dev"
}
```

### How to use?

**Create a new site**:

```bash
$ spress site:new /your-site-dir directive
$ cd /your-site-dir directive
$ spress site:build --server --watch
```

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
```
---
comments: false
---
```
