---
description: GetMacieSessionResponse schema from Amazon Macie API
layout: schema
name: GetMacieSessionResponse
properties_list:
- description: ''
  name: createdAt
  type: object
- description: ''
  name: findingPublishingFrequency
  type: object
- description: ''
  name: serviceRole
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-macie-session-response-schema.json
slug: amazon-macie-get-macie-session-response
source_filename: amazon-macie-get-macie-session-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-macie-session-response-schema.json\",\n  \"title\": \"GetMacieSessionResponse\",\n  \"description\": \"GetMacieSessionResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the Amazon Macie account was created.\"\n        }\n      ]\n    },\n    \"findingPublishingFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingPublishingFrequency\"\n        },\n        {\n          \"description\": \"The frequency with which Amazon Macie publishes updates to policy findings for the account. This includes\
  \ publishing updates to Security Hub and Amazon EventBridge (formerly Amazon CloudWatch Events).\"\n        }\n      ]\n    },\n    \"serviceRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service-linked role that allows Amazon Macie to monitor and analyze data in Amazon Web Services resources for the account.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacieStatus\"\n        },\n        {\n          \"description\": \"The current status of the Amazon Macie account. Possible values are: PAUSED, the account is enabled but all Macie activities are suspended (paused) for the account; and, ENABLED, the account is enabled and all Macie activities are enabled for the account.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, of the most recent change to the status of the Amazon Macie account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-macie-session-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetMacieSessionResponse
---
