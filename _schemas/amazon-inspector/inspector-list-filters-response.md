---
description: ListFiltersResponse schema
layout: schema
name: ListFiltersResponse
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-filters-response-schema.json
slug: inspector-list-filters-response
source_filename: inspector-list-filters-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-filters-response-schema.json\",\n  \"title\": \"ListFiltersResponse\",\n  \"description\": \"ListFiltersResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \"Contains details on the filters associated with your account.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the <code>NextToken</code> value returned\
  \ from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"filters\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-filters-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListFiltersResponse
---
