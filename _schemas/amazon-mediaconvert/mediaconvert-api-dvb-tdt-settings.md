---
description: Use these settings to insert a DVB Time and Date Table (TDT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.
layout: schema
name: DvbTdtSettings
properties_list:
- description: ''
  name: TdtInterval
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-tdt-settings-schema.json
slug: mediaconvert-api-dvb-tdt-settings
source_filename: mediaconvert-api-dvb-tdt-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-tdt-settings-schema.json\",\n  \"title\": \"DvbTdtSettings\",\n  \"description\": \"Use these settings to insert a DVB Time and Date Table (TDT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TdtInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000Max30000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tdtInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-tdt-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbTdtSettings
---
