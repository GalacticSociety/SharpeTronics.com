source "https://rubygems.org"
# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!
gem "jekyll", "~> 4.2.2"
# This is the default theme for new Jekyll sites. You may change this to anything you like.
# gem "minima", "~> 2.5"

# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update github-pages`.
# gem "github-pages", group: :jekyll_plugins
# If you have any plugins, put them here!

group :jekyll_plugins do
   gem 'jekyll-feed', '~> 0.12'
   gem 'jekyll-menus'
   gem 'jekyll-tagging'
   gem 'jekyll-archives'
   gem 'jekyll-paginate-v2'
end

group :dev_plugins do
  gem 'webrick', '~> 1.7' # dep for Jekyll 4.2.2; Ruby 3 doesn't have webrick by default anymore.
  gem 'json', '~> 2.1' # dep for transforming json data
  gem 'faraday' # a simple, but flexible HTTP client library, with support for multiple backends.
  gem 'httpx' # swiss army knife of Ruby for HTTP
  gem 'faraday-multipart' # send with UDP; No encoding of the data
  gem 'rails' # must use Rails for .blank support
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
install_if -> { RUBY_PLATFORM =~ %r!mingw|mswin|java! } do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :install_if => Gem.win_platform?
