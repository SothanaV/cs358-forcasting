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

# unmount
fusermount -u /path/to/mount
```