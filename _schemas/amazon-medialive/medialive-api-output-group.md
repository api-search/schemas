---
description: Output groups for this Live Event. Output groups contain information about where streams should be distributed.
layout: schema
name: OutputGroup
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: OutputGroupSettings
  type: object
- description: ''
  name: Outputs
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-output-group-schema.json
slug: medialive-api-output-group
source_filename: medialive-api-output-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-group-schema.json\",\n  \"title\": \"OutputGroup\",\n  \"description\": \"Output groups for this Live Event. Output groups contain information about where streams should be distributed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Custom output group name optionally defined by the user.\"\n        }\n      ]\n    },\n    \"OutputGroupSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputGroupSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputGroupSettings\"\n          },\n   \
  \       \"description\": \"Settings associated with the output group.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Outputs\",\n    \"OutputGroupSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-output-group-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputGroup
---
