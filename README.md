# heroku-play-store-application-credentials-buildpack
Generates a play store service account credential file based on Heroku Config Vars.

This repository is a fork from [elishaterada/heroku-google-application-credentials-buildpack](https://github.com/elishaterada/heroku-google-application-credentials-buildpack). It fixes some bugs that I found during my usage of the original repository.

## Usage

1. Create Config Vars key `PLAY_STORE_CREDENTIALS` and paste the content of service account credential JSON file as is.
2.  Create a key under Config Vars `PLAY_STORE_CREDENTIALS_FILE` and set a value as `play-store-credentials.json`.

The script will generate a file called `play-store-credentials.json` which holds the key from the step #1 above. Use this file to configure things.
