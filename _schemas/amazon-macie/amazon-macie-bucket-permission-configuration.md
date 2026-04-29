---
description: Provides information about the account-level and bucket-level permissions settings for an S3 bucket.
layout: schema
name: BucketPermissionConfiguration
properties_list:
- description: ''
  name: accountLevelPermissions
  type: object
- description: ''
  name: bucketLevelPermissions
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-permission-configuration-schema.json
slug: amazon-macie-bucket-permission-configuration
source_filename: amazon-macie-bucket-permission-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-permission-configuration-schema.json\",\n  \"title\": \"BucketPermissionConfiguration\",\n  \"description\": \"Provides information about the account-level and bucket-level permissions settings for an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountLevelPermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountLevelPermissions\"\n        },\n        {\n          \"description\": \"The account-level permissions settings that apply to the bucket.\"\n        }\n      ]\n    },\n    \"bucketLevelPermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketLevelPermissions\"\n        },\n        {\n          \"description\": \"The bucket-level permissions settings for the bucket.\"\n    \
  \    }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-permission-configuration-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketPermissionConfiguration
---
