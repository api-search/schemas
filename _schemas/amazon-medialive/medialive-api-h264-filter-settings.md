---
description: H264 Filter Settings
layout: schema
name: H264FilterSettings
properties_list:
- description: ''
  name: TemporalFilterSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-h264-filter-settings-schema.json
slug: medialive-api-h264-filter-settings
source_filename: medialive-api-h264-filter-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h264-filter-settings-schema.json\",\n  \"title\": \"H264FilterSettings\",\n  \"description\": \"H264 Filter Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TemporalFilterSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemporalFilterSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"temporalFilterSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-h264-filter-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H264FilterSettings
---
