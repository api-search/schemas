---
description: Provides a subset of information about an allow list.
layout: schema
name: AllowListSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-allow-list-summary-schema.json
slug: amazon-macie-allow-list-summary
source_filename: amazon-macie-allow-list-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-summary-schema.json\",\n  \"title\": \"AllowListSummary\",\n  \"description\": \"Provides a subset of information about an allow list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin71Max89PatternArnAwsAwsCnAwsUsGovMacie2AZ19920D12AllowListAZ0922\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the allow list.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the allow list was created in Amazon Macie.\"\n        }\n      ]\n    },\n\
  \    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max512PatternSS\"\n        },\n        {\n          \"description\": \"The custom description of the allow list.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin22Max22PatternAZ0922\"\n        },\n        {\n          \"description\": \"The unique identifier for the allow list.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max128Pattern\"\n        },\n        {\n          \"description\": \"The custom name of the allow list.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the allow list's settings were\
  \ most recently changed in Amazon Macie.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-allow-list-summary-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AllowListSummary
---
