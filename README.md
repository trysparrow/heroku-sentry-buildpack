# heroku-sentry-buildpack
Buildpack for pushing releases into sentry.

## Requirements

You need to set these environment variables on the application where the builpack will run:
```
SENTRY_AUTH_TOKEN
SENTRY_ORG
SENTRY_PROJECT
```

## Adding this buildpack to the application
- Go to Applicatoin -> settings -> buildpacks
- Add the full github url for this repo as a buildpack
- Add this buildpack after the buildpacks that add node/python as it requires node to install sentry-cli
