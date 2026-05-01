---
description: Provides information about an Amazon Web Services account and entity that performed an action on an affected resource. The action was performed using the credentials for an Amazon Web Services account other than your own account.
layout: schema
name: AwsAccount
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: principalId
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-aws-account-schema.json
slug: amazon-macie-aws-account
source_filename: amazon-macie-aws-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-aws-account-schema.json\",\n  \"title\": \"AwsAccount\",\n  \"description\": \"Provides information about an Amazon Web Services account and entity that performed an action on an affected resource. The action was performed using the credentials for an Amazon Web Services account other than your own account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"principalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the entity\
  \ that performed the action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-aws-account-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AwsAccount
---
