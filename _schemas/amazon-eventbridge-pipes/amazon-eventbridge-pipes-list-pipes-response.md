---
description: ListPipesResponse schema from Amazon EventBridge Pipes
layout: schema
name: ListPipesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Pipes
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-list-pipes-response-schema.json
slug: amazon-eventbridge-pipes-list-pipes-response
source_filename: amazon-eventbridge-pipes-list-pipes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-list-pipes-response-schema.json\",\n  \"title\": \"ListPipesResponse\",\n  \"description\": \"ListPipesResponse schema from Amazon EventBridge Pipes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If <code>nextToken</code> is returned, there are more results available. The value of <code>nextToken</code> is a unique pagination token for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return an HTTP 400 InvalidToken error.\"\n        }\n      ]\n    },\n  \
  \  \"Pipes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeList\"\n        },\n        {\n          \"description\": \"The pipes returned by the call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-list-pipes-response-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: ListPipesResponse
---
