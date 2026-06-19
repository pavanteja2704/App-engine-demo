# App-engine-demo

Step 1: Install Google Cloud SDK

Verify installation:
gcloud --version

Login:
gcloud auth login

Step 3: Set Project

Check projects:
gcloud projects list

Set project:
gcloud config set project PROJECT_ID

Example:
gcloud config set project my-webapp-project

Verify:
gcloud config list

Step 4: Enable App Engine API
gcloud services enable appengine.googleapis.com

Step 5: Create App Engine Application

If App Engine is not created yet:
gcloud app create --region=asia-south1

Choose a region close to you:
asia-south1 (Mumbai)
asia-southeast1 (Singapore)

⚠️ App Engine region cannot be changed later.

Step 6: Navigate to Project Folder
cd webapp

Verify:
ls

You should see:
assets
js
style
index.html
app.yaml

Step 7: Deploy
gcloud app deploy

When prompted:
Do you want to continue (Y/n)?

Enter:
Y

Wait for deployment to complete.

Step 8: Open Website
gcloud app browse
or
gcloud app describe

You'll get a URL like:
https://PROJECT_ID.uc.r.appspot.com
