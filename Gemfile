source "https://rubygems.org"

# GitHub Pages environment
gem "github-pages", group: :jekyll_plugins

# Core Jekyll
gem "jekyll", "~> 3.9"   # GitHub Pages currently uses Jekyll 3.9.x

# Plugins supported by GitHub Pages (safe mode)
gem "jekyll-feed", group: :jekyll_plugins
gem "jekyll-seo-tag", group: :jekyll_plugins
gem "jekyll-sitemap", group: :jekyll_plugins
gem "jekyll-paginate", group: :jekyll_plugins

# Optional plugins (local use only, not supported on GitHub Pages)
group :jekyll_plugins do
  gem "jekyll-archives"   # For category/tag archive pages
end

# Development tools
group :development do
  gem "webrick", "~> 1.7"   # Needed for local Jekyll server in Ruby 3+
end
