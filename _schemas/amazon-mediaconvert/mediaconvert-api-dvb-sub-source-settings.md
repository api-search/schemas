---
description: DVB Sub Source Settings
layout: schema
name: DvbSubSourceSettings
properties_list:
- description: ''
  name: Pid
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-sub-source-settings-schema.json
slug: mediaconvert-api-dvb-sub-source-settings
source_filename: mediaconvert-api-dvb-sub-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sub-source-settings-schema.json\",\n  \"title\": \"DvbSubSourceSettings\",\n  \"description\": \"DVB Sub Source Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pid\"\n          },\n          \"description\": \"When using DVB-Sub with Burn-In or SMPTE-TT, use this PID for the source content. Unused for DVB-Sub passthrough. All DVB-Sub content is passed through, regardless of selectors.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sub-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSubSourceSettings
---
