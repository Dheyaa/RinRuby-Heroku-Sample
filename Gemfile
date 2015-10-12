source 'https://rubygems.org'

ruby '2.2.3'

# General
# ================================================
#
gem 'rails', '4.2.4'
gem 'exception_notification', '~> 4.0.1'

# R
# ================================================
#
gem 'rinruby'

# Database and Server
# ================================================
#
gem 'puma', '~> 2.9.1'
gem 'pg', '~> 0.17.1'

# Background Jobs
# ================================================
#
gem 'sidekiq', '~> 3.3.0'
# This gives us sidekiq web interface
# if you require 'sinatra' you get the DSL extended to Object
gem 'sinatra', :require => nil

# Heroku
# ================================================
#
group :production do
  gem 'rails_12factor'
end


# General Development and Test Gems
# ================================================
#
group :development do
  gem 'json_spec', '~> 1.1.4'
  gem 'guard', '~> 2.12.5'
  gem 'guard-jslint-on-rails'
  gem 'guard-rspec', '~> 4.5.0'
  gem 'binding_of_caller', :platforms=>[:mri_19, :rbx]
  gem 'meta_request'
  gem 'bullet'
  gem 'brakeman'
  gem 'rails_best_practices'
  gem 'annotate'
  gem 'letter_opener'
  gem 'better_errors'
  gem 'rubocop'
end

group :development, :test do
  gem 'rspec-rails', '~> 3.1.0'
  gem 'rspec-its'
  gem 'spring-commands-rspec'
  gem 'database_cleaner', '~> 1.3.0'
  # gem "jazz_hands", :git => 'https://github.com/xcskier56/jazz_hands.git'
  gem 'jazz_hands', github: 'nixme/jazz_hands', branch: 'bring-your-own-debugger'
  gem 'pry-byebug', '~> 1.3.2' # behind latest version b/c jazz_hands needs pry 0.9 and this is the only way to have them not conflict.
  gem 'timecop', '~> 0.7.1'
  gem 'faker', '~> 1.4.3'
  gem 'factory_girl_rails', '~> 4.4.1'
end

group :test do
  gem 'ruby-prof'
  gem 'test-unit'
  gem 'capybara'
  gem 'capybara-webkit'
  gem 'jasmine'
  gem 'test_after_commit'
  gem 'shoulda-matchers', require: false
end
