# cs358-project

Potential and Demand of Import Export goods on Google cloud platform

# copy file to gcp storage
```
gsutil -m cp -r dir gs://my-bucket
```
# delete 
```
gsutil -m rm -r gs://cs358-project/original_dataset_customs
```

# mount ai platform to gcp scorage
ref https://github.com/GoogleCloudPlatform/gcsfuse/

```
gcloud auth login

# mount
gcsfuse --implicit-dirs <my-bucket> </path/to/mount>

gcsfuse --implicit-dirs cs358-project ./bucket


# unmount
fusermount -u /path/to/mount
```

# git crash
```
rm -f .git/index.lock
```

# insert data to BQ

insert data<br>
ref https://cloud.google.com/bigquery/streaming-data-into-bigquery

create schema<br>
ref https://cloud.google.com/bigquery/docs/tables

# query data in BQ
ref https://cloud.google.com/bigquery/docs/quickstarts/quickstart-client-libraries

# sklearn
partial_fit<br>
ref https://scikit-learn.org/0.15/modules/scaling_strategies.html