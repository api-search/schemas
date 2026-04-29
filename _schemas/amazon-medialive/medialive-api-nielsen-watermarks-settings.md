---
description: Nielsen Watermarks Settings
layout: schema
name: NielsenWatermarksSettings
properties_list:
- description: ''
  name: NielsenCbetSettings
  type: object
- description: ''
  name: NielsenDistributionType
  type: object
- description: ''
  name: NielsenNaesIiNwSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-nielsen-watermarks-settings-schema.json
slug: medialive-api-nielsen-watermarks-settings
source_filename: medialive-api-nielsen-watermarks-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-watermarks-settings-schema.json\",\n  \"title\": \"NielsenWatermarksSettings\",\n  \"description\": \"Nielsen Watermarks Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NielsenCbetSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenCBET\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenCbetSettings\"\n          },\n          \"description\": \"Complete these fields only if you want to insert watermarks of type Nielsen CBET\"\n        }\n      ]\n    },\n    \"NielsenDistributionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenWatermarksDistributionTypes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenDistributionType\"\
  \n          },\n          \"description\": \"Choose the distribution types that you want to assign to the watermarks:\\n- PROGRAM_CONTENT\\n- FINAL_DISTRIBUTOR\"\n        }\n      ]\n    },\n    \"NielsenNaesIiNwSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenNaesIiNw\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenNaesIiNwSettings\"\n          },\n          \"description\": \"Complete these fields only if you want to insert watermarks of type Nielsen NAES II (N2) and Nielsen NAES VI (NW).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-watermarks-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NielsenWatermarksSettings
---
