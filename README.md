# MaterialDocs

MaterialDocs is a material two-column Jekyll theme designed for documentation websites.  It is built with [Material Design Lite](https://getmdl.io).

## Installation

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

## Usage

MaterialDocs supports a few optional custom values in the YAML front matter.
```yaml
menu: Example Page # will use this as the menu item text instead of title
parent: index.md # will make this menu item a child of the index.md item
weight: 2 # smaller weights rise to the top of the menu
```

MaterialDocs also supports changing the color scheme by setting `mdl_colors` in _config.yml to a supported Material Design Lite scheme (e.g. indigo-pink, deep_orange-blue).  Use the [MDL theme builder](https://getmdl.io/customize/index.html) to find color schemes.

The footer copyright notice may be overridden by setting `copyright` in _config.yml.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/chromatical/jekyll-materialdocs.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
