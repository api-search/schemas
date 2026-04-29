---
description: Provides information about the account-level permissions settings that apply to an S3 bucket.
layout: schema
name: AccountLevelPermissions
properties_list:
- description: ''
  name: blockPublicAccess
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-account-level-permissions-schema.json
slug: amazon-macie-account-level-permissions
source_filename: amazon-macie-account-level-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-account-level-permissions-schema.json\",\n  \"title\": \"AccountLevelPermissions\",\n  \"description\": \"Provides information about the account-level permissions settings that apply to an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blockPublicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockPublicAccess\"\n        },\n        {\n          \"description\": \"The block public access settings for the Amazon Web Services account that owns the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-account-level-permissions-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AccountLevelPermissions
---
