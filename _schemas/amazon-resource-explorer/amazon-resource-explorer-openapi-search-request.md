---
description: SearchRequest schema from openapi
layout: schema
name: SearchRequest
properties_list:
- description: A string that includes keywords and filters to search for resources.
  name: QueryString
  type: string
- description: The maximum number of results to include in the response.
  name: MaxResults
  type: integer
- description: The token for the next page of results.
  name: NextToken
  type: string
- description: The ARN of the view to search.
  name: ViewArn
  type: string
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
schema_file: json-schema/amazon-resource-explorer-openapi-search-request-schema.json
slug: amazon-resource-explorer-openapi-search-request
source_filename: amazon-resource-explorer-openapi-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-search-request-schema.json\",\n  \"title\": \"SearchRequest\",\n  \"description\": \"SearchRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueryString\": {\n      \"type\": \"string\",\n      \"description\": \"A string that includes keywords and filters to search for resources.\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to include in the response.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the next page of results.\"\n    },\n    \"ViewArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the view to search.\"\n    }\n  },\n  \"required\": [\n    \"QueryString\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/json-schema/amazon-resource-explorer-openapi-search-request-schema.json
tags:
- AWS
- Discovery
- Inventory
- Operations
- Resource Management
title: SearchRequest
---
