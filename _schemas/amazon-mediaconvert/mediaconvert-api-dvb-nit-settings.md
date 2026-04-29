---
description: Use these settings to insert a DVB Network Information Table (NIT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.
layout: schema
name: DvbNitSettings
properties_list:
- description: ''
  name: NetworkId
  type: object
- description: ''
  name: NetworkName
  type: object
- description: ''
  name: NitInterval
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-nit-settings-schema.json
slug: mediaconvert-api-dvb-nit-settings
source_filename: mediaconvert-api-dvb-nit-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-nit-settings-schema.json\",\n  \"title\": \"DvbNitSettings\",\n  \"description\": \"Use these settings to insert a DVB Network Information Table (NIT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkId\"\n          },\n          \"description\": \"The numeric value placed in the Network Information Table (NIT).\"\n        }\n      ]\n    },\n    \"NetworkName\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkName\"\n          },\n          \"description\": \"The network name text placed in the network_name_descriptor inside the Network Information Table. Maximum length is 256 characters.\"\n        }\n      ]\n    },\n    \"NitInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin25Max10000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nitInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-nit-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbNitSettings
---
