---
description: Provides information about the permissions settings of the bucket policy for an S3 bucket.
layout: schema
name: BucketPolicy
properties_list:
- description: ''
  name: allowsPublicReadAccess
  type: object
- description: ''
  name: allowsPublicWriteAccess
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-policy-schema.json
slug: amazon-macie-bucket-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-policy-schema.json\",\n  \"title\": \"BucketPolicy\",\n  \"description\": \"Provides information about the permissions settings of the bucket policy for an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowsPublicReadAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the bucket policy allows the general public to have read access to the bucket.\"\n        }\n      ]\n    },\n    \"allowsPublicWriteAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the bucket policy allows the general public to have write access to the bucket.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-policy-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketPolicy
---
