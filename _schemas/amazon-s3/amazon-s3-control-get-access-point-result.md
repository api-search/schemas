---
description: ''
layout: schema
name: GetAccessPointResult
properties_list:
- description: The name of the access point.
  name: Name
  type: string
- description: The name of the bucket associated with the access point.
  name: Bucket
  type: string
- description: Indicates whether this access point allows access from the public internet.
  name: NetworkOrigin
  type: string
- description: ''
  name: VpcConfiguration
  type: object
- description: The date and time when the access point was created.
  name: CreationDate
  type: string
- description: The alias for the access point.
  name: Alias
  type: string
- description: The ARN for the access point.
  name: AccessPointArn
  type: string
- description: ''
  name: Endpoints
  type: object
- description: The AWS account ID associated with the S3 bucket.
  name: BucketAccountId
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-get-access-point-result-schema.json
slug: amazon-s3-control-get-access-point-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetAccessPointResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the access point.\"\n    },\n    \"Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket associated with the access point.\"\n    },\n    \"NetworkOrigin\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether this access point allows access from the public internet.\"\n    },\n    \"VpcConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the access point was created.\"\n    },\n    \"Alias\": {\n      \"type\": \"string\",\n      \"description\": \"The alias for the access point.\"\n    },\n    \"AccessPointArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN for\
  \ the access point.\"\n    },\n    \"Endpoints\": {\n      \"type\": \"object\"\n    },\n    \"BucketAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account ID associated with the S3 bucket.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-get-access-point-result-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: GetAccessPointResult
---
