---
description: Static Key Settings
layout: schema
name: StaticKeySettings
properties_list:
- description: ''
  name: KeyProviderServer
  type: object
- description: ''
  name: StaticKeyValue
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-static-key-settings-schema.json
slug: medialive-api-static-key-settings
source_filename: medialive-api-static-key-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-static-key-settings-schema.json\",\n  \"title\": \"StaticKeySettings\",\n  \"description\": \"Static Key Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyProviderServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyProviderServer\"\n          },\n          \"description\": \"The URL of the license server used for protecting content.\"\n        }\n      ]\n    },\n    \"StaticKeyValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin32Max32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"staticKeyValue\"\n          },\n          \"description\": \"Static key value as a 32 character hexadecimal\
  \ string.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StaticKeyValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-static-key-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: StaticKeySettings
---
