---
description: ListAccessPreviewsResponse schema from AWS IAM Access Analyzer API
layout: schema
name: ListAccessPreviewsResponse
properties_list:
- description: ''
  name: accessPreviews
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-access-previews-response-schema.json
slug: iam-access-analyzer-list-access-previews-response
source_filename: iam-access-analyzer-list-access-previews-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-access-previews-response-schema.json\",\n  \"title\": \"ListAccessPreviewsResponse\",\n  \"description\": \"ListAccessPreviewsResponse schema from AWS IAM Access Analyzer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPreviews\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPreviewsList\"\n        },\n        {\n          \"description\": \"A list of access previews retrieved for the analyzer.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessPreviews\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-access-previews-response-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ListAccessPreviewsResponse
---
