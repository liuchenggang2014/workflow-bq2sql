# workflow-bq2sql

## Pre-requirement
1. create the bq table with the schema
2. create the cloud sql databases and table with the same schema of bq
3. create a service account with project editor role

## steps:

1. edit the workflow's var's to fit your project/cloudsql/query/...
2. run command
```
gcloud workflows deploy --source=./bq2sql.yaml --location=us-central1 --service-account=sa-email bq2sql

gcloud workflows run bq2sql
```

