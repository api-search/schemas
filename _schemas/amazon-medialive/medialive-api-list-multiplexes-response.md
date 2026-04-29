---
description: Placeholder documentation for ListMultiplexesResponse
layout: schema
name: ListMultiplexesResponse
properties_list:
- description: ''
  name: Multiplexes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-multiplexes-response-schema.json
slug: medialive-api-list-multiplexes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-multiplexes-response-schema.json\",\n  \"title\": \"ListMultiplexesResponse\",\n  \"description\": \"Placeholder documentation for ListMultiplexesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Multiplexes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMultiplexSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexes\"\n          },\n          \"description\": \"List of multiplexes.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Token for the next ListMultiplexes request.\"\n  \
  \      }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-multiplexes-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListMultiplexesResponse
---
