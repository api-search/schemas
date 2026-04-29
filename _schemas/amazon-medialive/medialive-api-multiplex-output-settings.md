---
description: Multiplex Output Settings
layout: schema
name: MultiplexOutputSettings
properties_list:
- description: ''
  name: Destination
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-output-settings-schema.json
slug: medialive-api-multiplex-output-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-output-settings-schema.json\",\n  \"title\": \"MultiplexOutputSettings\",\n  \"description\": \"Multiplex Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"Destination is a Multiplex.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexOutputSettings
---
