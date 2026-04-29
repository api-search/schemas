---
description: <p>Provides information about an account-related request that hasn't been processed.</p>
layout: schema
name: UnprocessedAccount
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-unprocessed-account-schema.json
slug: amazon-macie-unprocessed-account
source_filename: amazon-macie-unprocessed-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-unprocessed-account-schema.json\",\n  \"title\": \"UnprocessedAccount\",\n  \"description\": \" <p>Provides information about an account-related request that hasn't been processed.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account that the request applies to.\"\n        }\n      ]\n    },\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"The source of the issue or delay in processing the request.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The reason why the request hasn't been processed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-unprocessed-account-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UnprocessedAccount
---
