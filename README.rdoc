= redmine_doorkeeper

To run the local engine server:

```
bundle install
bundle exec rake doorkeeper:server
````

By default, it uses the latest Rails version with ActiveRecord. To run the
tests with a specific Rails version:

```
BUNDLE_GEMFILE=gemfiles/rails_6_0.gemfile bundle exec rake
```

Installation
Type below commands:

$ cd $RAILS_ROOT/plugins
$ git clone git://github.com/suer/redmine_oauth_provider.git
Create database tables:

rake redmine:plugins:migrate RAILS_ENV=production
Then, restart your Redmine.
