---
description: Retrieves a list of resources that have been analyzed.
layout: schema
name: ListAnalyzedResourcesRequest
properties_list:
- description: ''
  name: analyzerArn
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-list-analyzed-resources-request-schema.json
slug: iam-access-analyzer-list-analyzed-resources-request
source_filename: iam-access-analyzer-list-analyzed-resources-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-analyzed-resources-request-schema.json\",\n  \"title\": \"ListAnalyzedResourcesRequest\",\n  \"description\": \"Retrieves a list of resources that have been analyzed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analyzerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyzerArn\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-getting-started.html#permission-resources\\\">ARN of the analyzer</a> to retrieve a list of analyzed resources from.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"\
  The type of resource.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A token used for pagination of results returned.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The maximum number of results to return in the response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"analyzerArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-list-analyzed-resources-request-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: ListAnalyzedResourcesRequest
---
