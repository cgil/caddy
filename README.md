# Caddy - Case Study
Urban freedom through convenient affordable storage spread throughout the city.

This is a project I worked on after work and during weekends from January - March of 2017. The goal was to gain experience in speaking with customers, gathering requirements, building a landing page, and releasing it to customers.

I worked on this with Andrew acting as the primary engineer and later recruited three friends to help pitch the product and gather customer feedback. This culminated in "selling" Caddy to street vendors in Union Square and Williamsburg.

### Marketing, feedback, customer studies, designs, economics.
Documents overviewing the process, market potential, economics, and and customer feedback can be found in the `case_study_documents` folder.


## Development

### Bootstrap
```
# Set up your environment
$ cd caddy
$ virtualenv env
$ source env/bin/activate

$ pip install fabric  # If this is not already installed globally.
# Bootstrap dependencies
$ fab bootstrap
```

### Testing
```
# After bootstrapping
$ fab test
```

### Running locally
```
# Run a local server
fab serve
```

### Migrations on production (Heroku)
```
# Migrate to head.
heroku db upgrade head

# Upgrade +X revisions.
heroku db upgrade +1

# Downgrade -X revisions.
heroku db downgrade -1
```

### Deploying to Heroku
```
# Deploys on push.
$ git heroku push master
```
