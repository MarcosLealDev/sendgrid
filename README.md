# SendGrid 
Written on Phyton 3.8

## Backend to be sent to GCP Cloud Functions
Trigger point: recebe_requisicao

## Frontend to be sent to a bucket 
Make sure the files have the web attribute
<code>
gsutil web set -m index.html -e 404.html gs://tcb-gl-onb-<seu-nome>
</code>

And allow all users
<code>
gsutil iam ch allUsers:objectViewer gs://tcb-gl-onb-<seu-nome>
</code>
