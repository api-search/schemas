---
description: Temporal Filter Settings
layout: schema
name: TemporalFilterSettings
properties_list:
- description: ''
  name: PostFilterSharpening
  type: object
- description: ''
  name: Strength
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-temporal-filter-settings-schema.json
slug: medialive-api-temporal-filter-settings
source_filename: medialive-api-temporal-filter-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-temporal-filter-settings-schema.json\",\n  \"title\": \"TemporalFilterSettings\",\n  \"description\": \"Temporal Filter Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PostFilterSharpening\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemporalFilterPostFilterSharpening\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"postFilterSharpening\"\n          },\n          \"description\": \"If you enable this filter, the results are the following:\\n- If the source content is noisy (it contains excessive digital artifacts), the filter cleans up the source.\\n- If the source content is already clean, the filter tends to decrease the bitrate, especially when the rate control mode is QVBR.\"\n        }\n      ]\n    },\n    \"\
  Strength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemporalFilterStrength\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"strength\"\n          },\n          \"description\": \"Choose a filter strength. We recommend a strength of 1 or 2. A higher strength might take out good information, resulting in an image that is overly soft.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-temporal-filter-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TemporalFilterSettings
---
