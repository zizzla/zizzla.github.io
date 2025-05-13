source "https://rubygems.org"
gem 'jekyll', '~> 4.4', '>= 4.4.1'

# Ruby 3 no longer includes webrick, which is used for jekyll serve
gem 'webrick', '~> 1.9', '>= 1.9.1', group: :development


# If you have any plugins, put them here!
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
  gem "jekyll-sass-converter", "~> 3.0.0"
  gem 'jekyll-sitemap', '~> 1.4'  
  gem 'jekyll-seo-tag', '~> 2.8'
  gem 'jekyll-tailwindcss', '~> 0.7.0'
end

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", "~> 1.2"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
# do not have a Java counterpart.
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]

