# It's easy to add more libraries or choose different versions. Any libraries
# specified here will be installed and made available to your morph.io scraper.
# Find out more: https://morph.io/documentation/ruby

source "https://rubygems.org"

ruby "2.0.0"

gem "scraperwiki", git: "https://github.com/openaustralia/scraperwiki-ruby.git", branch: "morph_defaults"
gem "mechanize"
gem 'capybara'
gem 'selenium-webdriver'
capybara = Capybara::Session.new(:selenium_chrome_headless)
# Start scraping
capybara.visit("https://jobboerse.arbeitsagentur.de/vamJB/stellenangeboteFinden.html?execution=e1s1&_eventId_detailView&bencs=2qLFXoXZQkxu50sbY0koWR1G7GGX6yLqcYubHza2Ezo%2F6pMNdiOlt%2B0vejMz3nPj&bencs=SqpxIhm4O5n4QlkBejiO0C9J1%2Btk1IEyloUQY0NgecpqXQxI0K3xIWpnPP9k7IerdamdrUvAtqKnc%2BVEowpPaw%3D%3D&bencs=mtOs6dB6giy9aU9wsEwy8rJGJ7GbkXucMqUjSQ%2Bs7SC3Qf9MRUJdtlcYPwbVEsFyz2X1ObN5fGC05cdMm5wykg%3D%3D")
puts capybara.find("#eingabemaske .cf").text
