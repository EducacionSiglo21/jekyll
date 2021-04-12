# frozen_string_literal: true

source "https://rubygems.org"
gemspec

gem "jekyll", "3.8.5"

group :jekyll_plugins do
  gem "jekyll-feed", "0.6"
  gem "jekyll-paginate-v2", "2.0.0"
  gem "jekyll-redirect-from"
  gem "jekyll-sitemap"
end

require 'rbconfig'
  if RbConfig::CONFIG['target_os'] =~ /darwin(1[0-3])/i
    gem 'rb-fsevent', '<= 0.9.4'
  end
