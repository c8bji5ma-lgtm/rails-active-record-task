source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end

ruby '4.0.6'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '8.1.3'
# Use postgresql as the database for Active Record
gem 'pg', '~> 1.6'
# Use Puma as the app server
gem 'puma', '~> 7.2'
# Keep the existing Sprockets asset pipeline
gem 'sprockets-rails', '~> 3.5'
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '~> 5'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.7'
gem 'rails-i18n', '~> 8.1'


group :development, :test do
  gem 'debug', platforms: [:mri, :windows], require: 'debug/prelude'
  gem 'capybara', '>= 2.15'
  gem 'csv'
  gem 'selenium-webdriver'
  gem 'pry-rails'
  gem 'faker'
  gem 'rspec-rails', '~> 8.0'
  gem 'database_cleaner'
  gem 'factory_bot_rails'
end

group :development do
  gem 'web-console', '>= 3.3.0'
  gem 'listen', '~> 3.9'
  gem 'spring', '~> 4.7'
  gem 'spring-watcher-listen', '~> 2.1'
end

group :test do
  gem 'rails-controller-testing'
  gem 'shoulda-matchers'
end

gem 'tzinfo-data', platforms: [:windows, :jruby]
