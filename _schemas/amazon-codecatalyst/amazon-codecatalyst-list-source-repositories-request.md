---
description: ListSourceRepositoriesRequest schema from Amazon CodeCatalyst
layout: schema
name: ListSourceRepositoriesRequest
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-list-source-repositories-request-schema.json
slug: amazon-codecatalyst-list-source-repositories-request
source_filename: amazon-codecatalyst-list-source-repositories-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repositories-request-schema.json\",\n  \"title\": \"ListSourceRepositoriesRequest\",\n  \"description\": \"ListSourceRepositoriesRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListSourceRepositoriesRequestNextTokenString\"\n        },\n        {\n          \"description\": \"A token returned from a call to this API to indicate the next batch of results to return, if any.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListSourceRepositoriesRequestMaxResultsInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results to show\
  \ in a single call to this API. If the number of results is larger than the number you specified, the response will include a <code>NextToken</code> element, which you can use to obtain additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repositories-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListSourceRepositoriesRequest
---
