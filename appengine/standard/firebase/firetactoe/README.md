# Tic Tac Toe, using Firebase, on App Engine Standard

This sample shows how to use the [Firebase](https://firebase.google.com/)
realtime database to implement a simple Tic Tac Toe game on [Google App Engine
Standard](https://cloud.google.com/appengine).

## Setup

Make sure you have the [Google Cloud SDK](https://cloud.google.com/sdk/)
installed. You'll need this to test and deploy your App Engine app.

### Authentication

* Create a project in the [Firebase
  console](https://firebase.google.com/console)
* In the Overview section, click 'Add Firebase to your web app' and replace the
  contents of the file
  [`templates/_firebase_config.html`](templates/_firebase_config.html) with the
  given snippet. This provides credentials for the javascript client.
* For running the sample locally, run the following command:

        gcloud beta auth application-default login \
            --scopes=https://www.googleapis.com/auth/firebase.database,https://www.googleapis.com/auth/userinfo.email

    This will provide credentials to your local app server, that would normally
    be provided automatically in the App Engine environment.

### Install dependencies

Before running or deploying this application, install the dependencies using
[pip](http://pip.readthedocs.io/en/stable/):

    pip install -t lib -r requirements.txt

## Running the sample

    dev_appserver.py .

For more information on running or deploying the sample, see the [App Engine
Standard README](../../README.md).
