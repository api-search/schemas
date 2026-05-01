---
description: A request to update a program in a multiplex.
layout: schema
name: UpdateMultiplexProgramRequest
properties_list:
- description: ''
  name: MultiplexProgramSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-multiplex-program-request-schema.json
slug: medialive-api-update-multiplex-program-request
source_filename: medialive-api-update-multiplex-program-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-multiplex-program-request-schema.json\",\n  \"title\": \"UpdateMultiplexProgramRequest\",\n  \"description\": \"A request to update a program in a multiplex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MultiplexProgramSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexProgramSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexProgramSettings\"\n          },\n          \"description\": \"The new settings for a multiplex program.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-multiplex-program-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateMultiplexProgramRequest
---
