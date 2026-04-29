---
description: Avail Settings
layout: schema
name: AvailSettings
properties_list:
- description: ''
  name: Esam
  type: object
- description: ''
  name: Scte35SpliceInsert
  type: object
- description: ''
  name: Scte35TimeSignalApos
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-avail-settings-schema.json
slug: medialive-api-avail-settings
source_filename: medialive-api-avail-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-avail-settings-schema.json\",\n  \"title\": \"AvailSettings\",\n  \"description\": \"Avail Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Esam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Esam\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"esam\"\n          }\n        }\n      ]\n    },\n    \"Scte35SpliceInsert\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35SpliceInsert\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35SpliceInsert\"\n          }\n        }\n      ]\n    },\n    \"Scte35TimeSignalApos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35TimeSignalApos\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"scte35TimeSignalApos\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-avail-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvailSettings
---
