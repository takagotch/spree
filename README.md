### spree
before
https://github.com/spree/spree

after solidus
https://github.com/solidusio/solidus

```
gem 'solidus'
gem 'solidus_auth_devise'
bundle exec rails g spree:install
bundle exec rails g solidus:auth:install
bundle exec rake railties:install:migrations
bundle exec rake db:migrate
bundle exec rails s
curl http://localhost:3000/

gem 'solidus', github: 'solidusio/solidus'
rails g spree:install --migrate=false --sample=false --seed=false
bundle exec rake railties:install:migrations
bundle exec rake db:migrate
bundle exec rake db:seed
bundle exec rake spree_sample:load

git clone git://github.com/solidusio/solidus.git
cd solidus
bundle install
bundle exe rake sandbox
cd sandbox
rails server
bas build.sh

DB=mysql bash build.sh

cd core
bundle exec rspec

DB=postgresql bundle exec rspec
COVERAGE=true bundle exec rspec
```

```ruby
config.assets.debug = false

//= require turbolinks
//= require backend/app/assets/javascripts/spree/backend/turbolinks-integration.js

```

