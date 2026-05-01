---
description: ListDevEnvironmentsRequest schema from Amazon CodeCatalyst
layout: schema
name: ListDevEnvironmentsRequest
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-list-dev-environments-request-schema.json
slug: amazon-codecatalyst-list-dev-environments-request
source_filename: amazon-codecatalyst-list-dev-environments-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-dev-environments-request-schema.json\",\n  \"title\": \"ListDevEnvironmentsRequest\",\n  \"description\": \"ListDevEnvironmentsRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"Information about filters to apply to narrow the results returned in the list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListDevEnvironmentsRequestNextTokenString\"\n        },\n        {\n          \"description\": \"A token returned from a call to this API to indicate the next batch of results to return, if any.\"\n     \
  \   }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListDevEnvironmentsRequestMaxResultsInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to show in a single call to this API. If the number of results is larger than the number you specified, the response will include a <code>NextToken</code> element, which you can use to obtain additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-dev-environments-request-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListDevEnvironmentsRequest
---
