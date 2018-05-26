# MaterialDocs

**View this theme on [ThemeJekyll](https://themejekyll.github.io/theme/materialdocs/)**

![MaterialDocs Screenshot](screenshot.png)

MaterialDocs is a material two-column Jekyll theme designed for documentation websites.  It is built with [Material Design Lite](https://getmdl.io).

## Standard Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-materialdocs"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-materialdocs
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-materialdocs

## Using with GitHub Pages

MaterialDocs is compatible with [Jekyll Remote Theme](https://github.com/benbalter/jekyll-remote-theme).

Add the following to `_config.yml` to enable Jekyll Remote Theme.

```yaml
plugins:
  - jekyll-remote-theme
```

Add the following to `_config.yml` to use MaterialDocs.

```yaml
remote_theme: chromatical/jekyll-materialdocs
```

## Site Options
```yaml
logo: /path/to/logo.png # an absolute or relative image path to use as the site logo
mdl_colors: indigo-pink # a supported Material Design Lite color scheme
copyright: Your Name # will override the copyright notice (default is site title)
search: true # enabled by default, set to false to disable site search
menu_style: dropdown # will only show child menu items for the main item selected
```
MaterialDocs supports changing the color scheme by setting `mdl_colors` in _config.yml to a supported Material Design Lite scheme (e.g. indigo-pink, deep_orange-blue).  Use the [MDL theme builder](https://getmdl.io/customize/index.html) to find color schemes.

## Front Matter Options

MaterialDocs supports a few optional custom values in the YAML front matter.
```yaml
menu: Example Page # will use this as the menu item text instead of title, set to false to remove from menu
tab: true # will open this page in a new tab
parent: index.md # will make this menu item a child of the index.md item
weight: 2 # smaller weights rise to the top of the menu
mdl_colors: deep_orange-blue # override global color scheme for this page
search: false # hides this page from search results
```

## Menu Data File

MaterialDocs supports data-driven menus in `_data/nav.yml`.  This can be used to add custom or external links to the menu.  Data-driven menu items support all menu-related YAML front matter options.  Additionally, data-driven menu items support the `id` option, which can be referenced in `parent`.  An example `nav.yml` is shown here.

```yaml
- title: "External Menu Item"
  url: "https://example.com"
  tab: true # opens this link in a new tab
  id: example # will be used as a parent item

- title: "Child Menu Item"
  url: "https://example.com"
  parent: example # will make this item a child of the item above (not displayed when menu_style is set to 'dropdown')

- title: "Another Child Menu Item"
  url: "https://example.com"
  parent: about.md # will make this item a child of the about.md item
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/chromatical/jekyll-materialdocs.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
