---
description: The response to the request.
layout: schema
name: ListAnalyzedResourcesResponse
properties_list:
- description: ''
  name: analyzedResources
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-analyzed-resources-response-schema.json
slug: iam-access-analyzer-list-analyzed-resources-response
source_filename: iam-access-analyzer-list-analyzed-resources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-analyzed-resources-response-schema.json\",\n  \"title\": \"ListAnalyzedResourcesResponse\",\n  \"description\": \"The response to the request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzedResourcesList\"\n        },\n        {\n          \"description\": \"A list of resources that were analyzed.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzedResources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-analyzed-resources-response-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: ListAnalyzedResourcesResponse
---
