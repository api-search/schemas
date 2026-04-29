---
description: Response for listing environments.
layout: schema
name: ListEnvironmentsResponse
properties_list:
- description: If there are more than 25 items in the list, only the first 25 are returned.
  name: nextToken
  type: string
- description: The list of environment identifiers.
  name: environmentIds
  type: array
provider_name: Amazon Cloud9
provider_slug: amazon-cloud9
schema_file: json-schema/cloud9-list-environments-response-schema.json
slug: cloud9-list-environments-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-list-environments-response-schema.json\",\n  \"title\": \"ListEnvironmentsResponse\",\n  \"description\": \"Response for listing environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"If there are more than 25 items in the list, only the first 25 are returned.\"\n    },\n    \"environmentIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The list of environment identifiers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-list-environments-response-schema.json
tags:
- AWS
- Cloud9
- IDE
- Development
- Browser-Based
title: ListEnvironmentsResponse
---
