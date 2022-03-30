# SendGrid 
Written on Phyton 3.8

## Backend to be sent to GCP Cloud Functions
Trigger point: recebe_requisicao
Environment Variables:
- MOODLE_TOKEN
- MOODLE_SERVER
- SENDGRID_API_KEY

## Frontend to be sent to a bucket 
Make sure the files have the web attribute <br />
<code>
gsutil web set -m index.html -e 404.html gs://bucket
</code>

And allow all users <br />
<code>
gsutil iam ch allUsers:objectViewer gs://bucket
</code>

## Moodle
Get a Moodle running :-)
Use GCP > Deployment Manager > Deploy Marketplace Solution
