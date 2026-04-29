---
description: Specifies the details of an account to associate with an Amazon Macie administrator account.
layout: schema
name: AccountDetail
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: email
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-account-detail-schema.json
slug: amazon-macie-account-detail
source_filename: amazon-macie-account-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-account-detail-schema.json\",\n  \"title\": \"AccountDetail\",\n  \"description\": \"Specifies the details of an account to associate with an Amazon Macie administrator account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account.\"\n        }\n      ]\n    },\n    \"email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The email address for the account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"email\",\n    \"accountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-account-detail-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AccountDetail
---
