---
description: ListFindingAggregationsResponse schema
layout: schema
name: ListFindingAggregationsResponse
properties_list:
- description: ''
  name: aggregationType
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: responses
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-finding-aggregations-response-schema.json
slug: inspector-list-finding-aggregations-response
source_filename: inspector-list-finding-aggregations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-finding-aggregations-response-schema.json\",\n  \"title\": \"ListFindingAggregationsResponse\",\n  \"description\": \"ListFindingAggregationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationType\"\n        },\n        {\n          \"description\": \"The type of aggregation to perform.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the <code>NextToken</code>\
  \ value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    },\n    \"responses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregationResponseList\"\n        },\n        {\n          \"description\": \"Objects that contain the results of an aggregation operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"aggregationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-finding-aggregations-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListFindingAggregationsResponse
---
