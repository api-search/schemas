---
description: EnableMacieRequest schema from Amazon Macie API
layout: schema
name: EnableMacieRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: findingPublishingFrequency
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-enable-macie-request-schema.json
slug: amazon-macie-enable-macie-request
source_filename: amazon-macie-enable-macie-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-enable-macie-request-schema.json\",\n  \"title\": \"EnableMacieRequest\",\n  \"description\": \"EnableMacieRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive token that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"findingPublishingFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingPublishingFrequency\"\n        },\n        {\n          \"description\": \"Specifies how often to publish updates to policy findings for the account. This includes publishing updates to Security Hub and Amazon\
  \ EventBridge (formerly Amazon CloudWatch Events).\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacieStatus\"\n        },\n        {\n          \"description\": \"Specifies the new status for the account. To enable Amazon Macie and start all Macie activities for the account, set this value to ENABLED.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-enable-macie-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: EnableMacieRequest
---
