---
description: CreateAllowListResponse schema from Amazon Macie API
layout: schema
name: CreateAllowListResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-create-allow-list-response-schema.json
slug: amazon-macie-create-allow-list-response
source_filename: amazon-macie-create-allow-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-allow-list-response-schema.json\",\n  \"title\": \"CreateAllowListResponse\",\n  \"description\": \"CreateAllowListResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin71Max89PatternArnAwsAwsCnAwsUsGovMacie2AZ19920D12AllowListAZ0922\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the allow list.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin22Max22PatternAZ0922\"\n        },\n        {\n          \"description\": \"The unique identifier for the allow list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-allow-list-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateAllowListResponse
---
