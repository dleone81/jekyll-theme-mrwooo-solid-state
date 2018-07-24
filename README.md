# Jekill Theme MrWooo Solid State

Welcome to your new Jekyll theme! In this directory, you'll find the files you need to be able to package up your theme into a gem. Put your layouts in `_layouts`, your includes in `_includes`, your sass files in `_sass` and any other assets in `assets`.

To experiment with this code, add some sample content and run `bundle exec jekyll serve` – this directory is setup just like a Jekyll site!

This gem is a package of HTML5up.net/solid-state theme for Jekyll.
I've added new features ready to use as:

* Google Analytics script
* Google Tag Manager script
* Google Maps API Key script
* Open Graph support (all)
* Social Icons
* Menu support as native theme

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-theme-mrwooo-solid-state"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-mrwooo-solid-state
title: Solid state
short_description: This is Solid State
description: >- # this means to ignore newlines until "baseurl:"
  Another free + fully responsive site template by <a href="http://html5up.net">HTML5 UP</a>
baseurl: "/"

# google services
ganalytics:
gtagmanager:
gmapsapikey:

# facebook
fpixel:

# collections
collections:
  main:
    output: true
    permalink: /main/:name

  defaults:
  - scope:
      path: 'assets/images'
      type: 'main'
  values:
    image: true

# contacts
address: >-
  Untitled Inc  1234<br />Somewhere Road Suite 2894  Nashville,<br />TN 00000-0000
phone: (000) 000-0000
email: information@untitled.tld
  
# social
twitter: twitter.com/untitled-tld
facebook: facebook.com/untitled-tld
instagram: instagram.com/untitled-tld
linkedin: linkedin.com/untitled-tld
youtube: youtube.com/untitled-tld
googleplus: googleplus.com/untitled-tld
github: github.com/untitled-tld
dribbble: dribbble.com/untitled-tld

# copyright
owner: Company
version: 0.0.1
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-theme-mrwooo-solid-state

## Usage

### Add menu

Menu is provided using collection feature.

To add menu as Solid state theme follow these steps:
1. create folder _data in root folder project
1. create in _data folder menu.yml as below. If you'd like to add more item to menu add them to menu.yml file and create page in _main folder
1. create _main folder
1. create in _menu folder three different file like sample-1.md as below

```
# menu.yml file
main_menu: Menu
link:
- title: Home
  url: index.html

- title: Generic
  url: generic.html

- title: Elements
  url: elements.html
```

```
---
layout: page
title: Tempus adipiscing
description: Lorem ipsum dolor sit amet, etiam lorem adipiscing elit. Cras turpis ante, nullam sit amet turpis non, sollicitudin posuere urna. Mauris id tellus arcu. Nunc vehicula id nulla dignissim dapibus. Nullam ultrices, neque et faucibus viverra, ex nulla cursus.
permalink: /wordpress/plugins/
image: /assets/images/pic02.jpg
---
Lorem ipsum dolor sit amet, etiam lorem adipiscing elit. Cras turpis ante, nullam sit amet turpis non, sollicitudin posuere urna. Mauris id tellus arcu. Nunc vehicula id nulla dignissim dapibus. Nullam ultrices, neque et faucibus viverra, ex nulla cursus.
```

And then execute:

```
    $ bundle exec jekyll serve
```

done!

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/dleone81/jekyll-theme-solid-state/issues. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `jekyll-theme-mrwooo-solid-state.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

