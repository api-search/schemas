---
description: DVB Time and Date Table (SDT)
layout: schema
name: DvbTdtSettings
properties_list:
- description: ''
  name: RepInterval
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-dvb-tdt-settings-schema.json
slug: medialive-api-dvb-tdt-settings
source_filename: medialive-api-dvb-tdt-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-tdt-settings-schema.json\",\n  \"title\": \"DvbTdtSettings\",\n  \"description\": \"DVB Time and Date Table (SDT)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RepInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max30000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"repInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-tdt-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbTdtSettings
---
