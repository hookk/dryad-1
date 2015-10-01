source 'https://rubygems.org'

ruby "2.2.3"

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.2.4'
# Use mysql as the database for Active Record
#gem 'mysql2'
#gem 'mysql2', '~> 0.3.18'
# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.1.0'
# See https://github.com/sstephenson/execjs#readme for more supported runtimes
gem 'therubyracer', platforms: :ruby

# Use jquery as the JavaScript library
gem 'jquery-rails'
# Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
gem 'turbolinks'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.0'
# bundle exec rake doc:rails generates the API under doc/api.
gem 'sdoc', '~> 0.4.0', group: :doc

# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use Unicorn as the app server
# gem 'unicorn'

if File.exist?(File.join('..', 'stash_engine')) && ENV['LOCAL_ENGINES'] == 'true'
  gem 'stash_engine', :path => '../stash_engine'
else
  gem 'stash_engine', :git => 'https://github.com/CDLUC3/stash_engine.git', :branch => 'development'
end

if File.exist?(File.join('..', 'stash_datacite')) && ENV['LOCAL_ENGINES'] == 'true'
  gem 'stash_datacite', :path => '../stash_datacite'
else
  gem 'stash_datacite', :git => 'https://github.com/CDLUC3/stash_datacite.git', :branch => 'development'
end



# Use Capistrano for deployment
gem 'capistrano', '~> 3.1'
gem 'capistrano-rails', '~> 1.1'
gem 'capistrano-passenger'
gem 'passenger'

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug'

  # Access an IRB console on exception pages or by using <%= console %> in views
  gem 'web-console', '~> 2.0'

  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'

  #testing framework
  gem 'rspec-rails', '~> 3.0'

  #test coverage
  gem 'simplecov' # TODO do we care about the version?
  gem 'simplecov-console' # TODO do we care about the version?

end

