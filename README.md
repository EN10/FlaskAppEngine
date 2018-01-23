# Flask Hello World on Google App Engine

Based on:
* [Python App Engine Quickstart](https://cloud.google.com/appengine/docs/standard/python/quickstart#hello_world_code_review)
* [Flask Hello World on Heroku](https://github.com/EN10/PythonHeroku)
* [Flask Hello World on App Engine](https://github.com/GoogleCloudPlatform/python-docs-samples/tree/master/appengine/standard/flask/hello_world)

#### Create Project:
Create a new GCP project and App Engine application using the GCP Console   
* [Go To App Engine](https://console.cloud.google.com/projectselector/appengine/create?lang=python)

### Install SDK:

**Install Google Cloud SDK :**

    export CLOUD_SDK_REPO="cloud-sdk-$(lsb_release -c -s)"
    echo "deb http://packages.cloud.google.com/apt $CLOUD_SDK_REPO main" | sudo tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
    curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
    sudo apt-get update && sudo apt-get install google-cloud-sdk
    
[Ref](https://cloud.google.com/sdk/docs/#deb)

#### Login, Verify & Select Project:

    gcloud init

#### Deploy app

    gcloud app deploy