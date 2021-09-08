# SWBATs

- [ ] Students will be able to host their rails applications on Heroku
- [ ] Students will be able to set up cors policies

# Objectives

- [ ] Create a new rails project
- [ ] Set up cors
    - uncomment rack-cors gem
    - uncomment initializers/cors.rb file
    - set origin

# Resources

- Rails hosting guide - https://my.learn.co/courses/262/pages/deploying-a-rails-api-to-heroku?module_item_id=26735
- Upgrading your ruby version - https://satchel.works/@wclittle/how-to-upgrade-ruby-versions-within-your-ruby-on-rails-app
    - rvm install 2.7.4
    - rvm use 2.7.4
    - gem install bundler
    - Change ruby verison in gemfile
    - bundle update
- Configuring Cors - https://stackoverflow.com/questions/63107489/how-to-allow-cors-in-ruby-on-rails-6-api-backend-deployed-on-heroku (first answer)

- If you didn't use --database=postgresql
    - create a new rails app with the proper flags - rails new app-name --api --minimal --database=postgresql
    - Copy your migrations, seeds, routes, controllers
    - To simply upgrade (not recommend) 
        - https://medium.com/@virtual_khan/converting-rails-from-sqlite3-to-postgresql-d97023314a14
        - may work
        - may run into trouble when deploying