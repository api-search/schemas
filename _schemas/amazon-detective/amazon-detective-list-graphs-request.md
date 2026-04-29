---
description: Request to list behavior graphs
layout: schema
name: ListGraphsRequest
properties_list:
- description: For requests to get the next page of results. The pagination token from the previous request.
  name: NextToken
  type: string
- description: The maximum number of graphs to return at a time.
  name: MaxResults
  type: integer
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-graphs-request-schema.json
slug: amazon-detective-list-graphs-request
source_filename: amazon-detective-list-graphs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-graphs-request-schema.json\",\n  \"title\": \"ListGraphsRequest\",\n  \"description\": \"Request to list behavior graphs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"For requests to get the next page of results. The pagination token from the previous request.\",\n      \"example\": \"abc123token\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of graphs to return at a time.\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-graphs-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListGraphsRequest
---
