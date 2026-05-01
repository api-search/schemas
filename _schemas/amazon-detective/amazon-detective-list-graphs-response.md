---
description: Response from listing behavior graphs
layout: schema
name: ListGraphsResponse
properties_list:
- description: A list of behavior graphs that the account is an administrator account of.
  name: GraphList
  type: array
- description: If there are more behavior graphs remaining in the results, then this is the pagination token to use.
  name: NextToken
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-graphs-response-schema.json
slug: amazon-detective-list-graphs-response
source_filename: amazon-detective-list-graphs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-graphs-response-schema.json\",\n  \"title\": \"ListGraphsResponse\",\n  \"description\": \"Response from listing behavior graphs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphList\": {\n      \"type\": \"array\",\n      \"description\": \"A list of behavior graphs that the account is an administrator account of.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Graph\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"If there are more behavior graphs remaining in the results, then this is the pagination token to use.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-graphs-response-schema.json
tags:
- Forensics
- Investigation
- Security
title: ListGraphsResponse
---
