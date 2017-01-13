# emberjs-lab

I'm sorry, i press to much fast up-arrow and enter, which was... git reset --hard, so for now here is my checklist :(

# Install Ember
$ npm install -g ember-cli@2.10

# Create a New Application
$ ember new ember-quickstart

$ cd ember-quickstart
$ ember server

# Let's create a new template using the ember generate command.
$ ember generate template application

# Define a Route
$ ember generate route pets

result will be
installing route
  create app/routes/pets.js
  create app/templates/pets.hbs
updating router
  add route pets
installing route-test
  create tests/unit/routes/pets-test.js


# Create a UI Component
$ ember generate component pets-list

# Building For Production
ember build --env production


# Ember acceptance tests
ember g acceptance-test list-pets

# run ember test
ember test --server

# Installing addons:
## Mirage usefull for create HTTP fake data for acceptances http responses
$ ember install ember-cli-mirage

# now we create and adapter to the mirage endopoints , see JSONAPIAdapter
$ ember generate adapter application

# create a new model
ember g model pet

#Creating a Handlebars Helper 
ember g helper pet-property-type

# Deploying
rm -rf dist
ember build --environment=development
cd dist
cp index.html 200.html
surge funny-name.surge.sh



