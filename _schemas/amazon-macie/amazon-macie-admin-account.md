---
description: Provides information about the delegated Amazon Macie administrator account for an organization in Organizations.
layout: schema
name: AdminAccount
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-admin-account-schema.json
slug: amazon-macie-admin-account
source_filename: amazon-macie-admin-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-admin-account-schema.json\",\n  \"title\": \"AdminAccount\",\n  \"description\": \"Provides information about the delegated Amazon Macie administrator account for an organization in Organizations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminStatus\"\n        },\n        {\n          \"description\": \"The current status of the account as the delegated Amazon Macie administrator account for the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-admin-account-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AdminAccount
---
