---
description: ListWorldExportJobsResponse schema from openapi
layout: schema
name: ListWorldExportJobsResponse
properties_list:
- description: ''
  name: worldExportJobSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-list-world-export-jobs-response-schema.json
slug: amazon-robomaker-openapi-list-world-export-jobs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-world-export-jobs-response-schema.json\",\n  \"title\": \"ListWorldExportJobsResponse\",\n  \"description\": \"ListWorldExportJobsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"worldExportJobSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldExportJobSummaries\"\n        },\n        {\n          \"description\": \"Summary information for world export jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the previous paginated request did not return all of the remaining results, the response object's <code>nextToken</code> parameter value is\
  \ set to a token. To retrieve the next set of results, call <code>ListWorldExportJobsRequest</code> again and assign that token to the request object's <code>nextToken</code> parameter. If there are no remaining results, the previous response object's NextToken parameter is set to null. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"worldExportJobSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-world-export-jobs-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: ListWorldExportJobsResponse
---
