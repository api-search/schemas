---
description: ListWorldsResponse schema from openapi
layout: schema
name: ListWorldsResponse
properties_list:
- description: ''
  name: worldSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-list-worlds-response-schema.json
slug: amazon-robomaker-openapi-list-worlds-response
source_filename: amazon-robomaker-openapi-list-worlds-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-worlds-response-schema.json\",\n  \"title\": \"ListWorldsResponse\",\n  \"description\": \"ListWorldsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"worldSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldSummaries\"\n        },\n        {\n          \"description\": \"Summary information for worlds.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the previous paginated request did not return all of the remaining results, the response object's <code>nextToken</code> parameter value is set to a token. To retrieve the next set of results, call\
  \ <code>ListWorlds</code> again and assign that token to the request object's <code>nextToken</code> parameter. If there are no remaining results, the previous response object's NextToken parameter is set to null. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-worlds-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: ListWorldsResponse
---
