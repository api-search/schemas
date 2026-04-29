---
description: UpdateMacieSessionRequest schema from Amazon Macie API
layout: schema
name: UpdateMacieSessionRequest
properties_list:
- description: ''
  name: findingPublishingFrequency
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-macie-session-request-schema.json
slug: amazon-macie-update-macie-session-request
source_filename: amazon-macie-update-macie-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-macie-session-request-schema.json\",\n  \"title\": \"UpdateMacieSessionRequest\",\n  \"description\": \"UpdateMacieSessionRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingPublishingFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingPublishingFrequency\"\n        },\n        {\n          \"description\": \"Specifies how often to publish updates to policy findings for the account. This includes publishing updates to Security Hub and Amazon EventBridge (formerly Amazon CloudWatch Events).\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MacieStatus\"\n        },\n        {\n          \"description\": \"Specifies a new status\
  \ for the account. Valid values are: ENABLED, resume all Amazon Macie activities for the account; and, PAUSED, suspend all Macie activities for the account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-macie-session-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateMacieSessionRequest
---
