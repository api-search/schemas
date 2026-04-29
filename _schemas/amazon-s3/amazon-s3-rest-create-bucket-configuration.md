---
description: The configuration information for the bucket.
layout: schema
name: CreateBucketConfiguration
properties_list:
- description: Specifies the Region where the bucket will be created. If you do not specify a Region, the bucket is created in the us-east-1 Region.
  name: LocationConstraint
  type: string
- description: Specifies the location of the bucket.
  name: Location
  type: object
- description: Specifies the information about the bucket to create.
  name: Bucket
  type: object
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-create-bucket-configuration-schema.json
slug: amazon-s3-rest-create-bucket-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateBucketConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"The configuration information for the bucket.\",\n  \"properties\": {\n    \"LocationConstraint\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the Region where the bucket will be created. If you do not specify a Region, the bucket is created in the us-east-1 Region.\"\n    },\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the location of the bucket.\"\n    },\n    \"Bucket\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the information about the bucket to create.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-create-bucket-configuration-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CreateBucketConfiguration
---
