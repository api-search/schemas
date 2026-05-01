---
description: Placeholder documentation for ListInputsResponse
layout: schema
name: ListInputsResponse
properties_list:
- description: ''
  name: Inputs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-inputs-response-schema.json
slug: medialive-api-list-inputs-response
source_filename: medialive-api-list-inputs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-inputs-response-schema.json\",\n  \"title\": \"ListInputsResponse\",\n  \"description\": \"Placeholder documentation for ListInputsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputs\"\n          }\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-inputs-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListInputsResponse
---
