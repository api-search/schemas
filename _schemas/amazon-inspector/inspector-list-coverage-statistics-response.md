---
description: ListCoverageStatisticsResponse schema
layout: schema
name: ListCoverageStatisticsResponse
properties_list:
- description: ''
  name: countsByGroup
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: totalCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-coverage-statistics-response-schema.json
slug: inspector-list-coverage-statistics-response
source_filename: inspector-list-coverage-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-coverage-statistics-response-schema.json\",\n  \"title\": \"ListCoverageStatisticsResponse\",\n  \"description\": \"ListCoverageStatisticsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countsByGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountsList\"\n        },\n        {\n          \"description\": \"An array with the number for each group.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the <code>NextToken</code>\
  \ value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    },\n    \"totalCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total number for all groups.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"totalCounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-coverage-statistics-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListCoverageStatisticsResponse
---
