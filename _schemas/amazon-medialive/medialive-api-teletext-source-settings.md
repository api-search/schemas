---
description: Teletext Source Settings
layout: schema
name: TeletextSourceSettings
properties_list:
- description: ''
  name: OutputRectangle
  type: object
- description: ''
  name: PageNumber
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-teletext-source-settings-schema.json
slug: medialive-api-teletext-source-settings
source_filename: medialive-api-teletext-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-teletext-source-settings-schema.json\",\n  \"title\": \"TeletextSourceSettings\",\n  \"description\": \"Teletext Source Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputRectangle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionRectangle\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputRectangle\"\n          },\n          \"description\": \"Optionally defines a region where TTML style captions will be displayed\"\n        }\n      ]\n    },\n    \"PageNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pageNumber\"\n          },\n          \"description\": \"Specifies the teletext page\
  \ number within the data stream from which to extract captions. Range of 0x100 (256) to 0x8FF (2303). Unused for passthrough. Should be specified as a hexadecimal string with no \\\"0x\\\" prefix.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-teletext-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TeletextSourceSettings
---
