## redmine_doorkeeper

To run the local engine server:

```
bundle install --without development test
bundle exec rake doorkeeper:server
````

By default, it uses the latest Rails version with ActiveRecord. To run the
tests with a specific Rails version:

```
BUNDLE_GEMFILE=gemfiles/rails_6_0.gemfile bundle exec rake
```

Installation

Type below commands:
```
$ cd $RAILS_ROOT/plugins  
$ git clone https://github.com/jex-redmine/redmine_doorkeeper.git
```
Create database tables:
```
bundle exec rake redmine:plugins:migrate NAME=redmine_doorkeeper RAILS_ENV=production
```

Then, restart your Redmine.
