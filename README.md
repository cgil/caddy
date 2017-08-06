# caddy
Urban freedom through convenient, affordable storage spread throughout the city.


# Bootstrap
```
# Set up your environment
$ cd caddy
$ virtualenv env
$ source env/bin/activate

$ pip install fabric  # If this is not already installed globally.
# Bootstrap dependencies
$ fab bootstrap
```

# Testing
```
# After bootstrapping
$ fab test
```

# Running locally
```
# Run a local server
fab serve
```

# Migrations on production (Heroku)
```
# Migrate to head.
heroku db upgrade head

# Upgrade +X revisions.
heroku db upgrade +1

# Downgrade -X revisions.
heroku db downgrade -1
```

# Deploying to Heroku
```
# Deploys on push.
$ git heroku push master
```
