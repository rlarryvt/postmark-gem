source "http://rubygems.org"

# Specify your gem's dependencies in postmark.gemspec
gemspec

group :test do
  gem 'rspec', '~> 3.7'
  gem 'rspec-its', '~> 1.2'
  gem 'fakeweb', :git => 'https://github.com/chrisk/fakeweb.git'
  gem 'fakeweb-matcher'
  gem 'mime-types'
  gem 'activesupport'
  gem 'i18n', '~> 0.6.0'
  gem 'yajl-ruby', '~> 1.0', :platforms => [:mingw, :mswin, :ruby]
  # Require gem:
require 'postmark'

# Create an instance of Postmark::ApiClient:
client = Postmark::ApiClient.new('fdb5fc7a-f606-4de1-8156-ccf7f682a7be')

# Send an email:
client.deliver(
  from: 'director@cityhotelcafe.org',
  to: 'director@cityhotelcafe.org',
  subject: 'Hello from Postmark',
  html_body: '<strong>Hello</strong> dear Postmark user.',
  track_opens: true)
end
