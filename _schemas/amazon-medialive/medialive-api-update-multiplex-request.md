---
description: A request to update a multiplex.
layout: schema
name: UpdateMultiplexRequest
properties_list:
- description: ''
  name: MultiplexSettings
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-multiplex-request-schema.json
slug: medialive-api-update-multiplex-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-multiplex-request-schema.json\",\n  \"title\": \"UpdateMultiplexRequest\",\n  \"description\": \"A request to update a multiplex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MultiplexSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexSettings\"\n          },\n          \"description\": \"The new settings for a multiplex.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of the multiplex.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-multiplex-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateMultiplexRequest
---
