---
description: Key Provider Settings
layout: schema
name: KeyProviderSettings
properties_list:
- description: ''
  name: StaticKeySettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-key-provider-settings-schema.json
slug: medialive-api-key-provider-settings
source_filename: medialive-api-key-provider-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-key-provider-settings-schema.json\",\n  \"title\": \"KeyProviderSettings\",\n  \"description\": \"Key Provider Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StaticKeySettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StaticKeySettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"staticKeySettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-key-provider-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: KeyProviderSettings
---
