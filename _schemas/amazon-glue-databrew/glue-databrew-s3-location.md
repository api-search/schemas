---
description: Represents an Amazon S3 location (bucket name, bucket owner, and object key) where DataBrew can read input data, or write output from a job.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: BucketOwner
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-s3-location-schema.json
slug: glue-databrew-s3-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"Represents an Amazon S3 location (bucket name, bucket owner, and object key) where DataBrew can read input data, or write output from a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Bucket\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket name.\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The unique name of the object in the bucket.\"\n        }\n      ]\n    },\n    \"BucketOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketOwner\"\
  \n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the bucket owner.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Bucket\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-s3-location-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: S3Location
---
