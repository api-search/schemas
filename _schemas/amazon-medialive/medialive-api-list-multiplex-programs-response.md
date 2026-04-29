---
description: Placeholder documentation for ListMultiplexProgramsResponse
layout: schema
name: ListMultiplexProgramsResponse
properties_list:
- description: ''
  name: MultiplexPrograms
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-multiplex-programs-response-schema.json
slug: medialive-api-list-multiplex-programs-response
source_filename: medialive-api-list-multiplex-programs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-multiplex-programs-response-schema.json\",\n  \"title\": \"ListMultiplexProgramsResponse\",\n  \"description\": \"Placeholder documentation for ListMultiplexProgramsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MultiplexPrograms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMultiplexProgramSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexPrograms\"\n          },\n          \"description\": \"List of multiplex programs.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Token\
  \ for the next ListMultiplexProgram request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-multiplex-programs-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListMultiplexProgramsResponse
---
