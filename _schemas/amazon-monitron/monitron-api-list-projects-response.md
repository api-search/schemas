---
description: ListProjectsResponse schema from Amazon Monitron API
layout: schema
name: ListProjectsResponse
properties_list:
- description: A list of Monitron projects.
  name: items
  type: array
- description: A pagination token to retrieve the next set of results.
  name: nextToken
  type: string
provider_name: Amazon Monitron
provider_slug: amazon-monitron
schema_file: json-schema/monitron-api-list-projects-response-schema.json
slug: monitron-api-list-projects-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-list-projects-response-schema.json\",\n  \"title\": \"ListProjectsResponse\",\n  \"description\": \"ListProjectsResponse schema from Amazon Monitron API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"description\": \"A list of Monitron projects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Project\"\n      },\n      \"type\": \"array\"\n    },\n    \"nextToken\": {\n      \"description\": \"A pagination token to retrieve the next set of results.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-list-projects-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListProjectsResponse
---
