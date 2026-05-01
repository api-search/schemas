---
description: Provides information about the bucket-level permissions settings for an S3 bucket.
layout: schema
name: BucketLevelPermissions
properties_list:
- description: ''
  name: accessControlList
  type: object
- description: ''
  name: blockPublicAccess
  type: object
- description: ''
  name: bucketPolicy
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-level-permissions-schema.json
slug: amazon-macie-bucket-level-permissions
source_filename: amazon-macie-bucket-level-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-level-permissions-schema.json\",\n  \"title\": \"BucketLevelPermissions\",\n  \"description\": \"Provides information about the bucket-level permissions settings for an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessControlList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlList\"\n        },\n        {\n          \"description\": \"The permissions settings of the access control list (ACL) for the bucket. This value is null if an ACL hasn't been defined for the bucket.\"\n        }\n      ]\n    },\n    \"blockPublicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockPublicAccess\"\n        },\n        {\n          \"description\": \"The block public access settings for the bucket.\"\
  \n        }\n      ]\n    },\n    \"bucketPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketPolicy\"\n        },\n        {\n          \"description\": \"The permissions settings of the bucket policy for the bucket. This value is null if a bucket policy hasn't been defined for the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-level-permissions-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketLevelPermissions
---
