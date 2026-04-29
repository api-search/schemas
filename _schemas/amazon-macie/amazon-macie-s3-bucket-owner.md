---
description: Provides information about the Amazon Web Services account that owns an S3 bucket.
layout: schema
name: S3BucketOwner
properties_list:
- description: ''
  name: displayName
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-bucket-owner-schema.json
slug: amazon-macie-s3-bucket-owner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-owner-schema.json\",\n  \"title\": \"S3BucketOwner\",\n  \"description\": \"Provides information about the Amazon Web Services account that owns an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The display name of the account that owns the bucket.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The canonical user ID for the account that owns the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-owner-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3BucketOwner
---
