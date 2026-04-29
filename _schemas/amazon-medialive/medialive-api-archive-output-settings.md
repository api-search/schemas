---
description: Archive Output Settings
layout: schema
name: ArchiveOutputSettings
properties_list:
- description: ''
  name: ContainerSettings
  type: object
- description: ''
  name: Extension
  type: object
- description: ''
  name: NameModifier
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-archive-output-settings-schema.json
slug: medialive-api-archive-output-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-archive-output-settings-schema.json\",\n  \"title\": \"ArchiveOutputSettings\",\n  \"description\": \"Archive Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArchiveContainerSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containerSettings\"\n          },\n          \"description\": \"Settings specific to the container type of the file.\"\n        }\n      ]\n    },\n    \"Extension\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"extension\"\n          },\n          \"description\": \"Output file extension. If excluded, this\
  \ will be auto-selected from the container type.\"\n        }\n      ]\n    },\n    \"NameModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nameModifier\"\n          },\n          \"description\": \"String concatenated to the end of the destination filename.  Required for multiple outputs of the same type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-archive-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ArchiveOutputSettings
---
