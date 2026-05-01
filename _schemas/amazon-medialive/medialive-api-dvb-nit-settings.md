---
description: DVB Network Information Table (NIT)
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
  name: RepInterval
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-dvb-nit-settings-schema.json
slug: medialive-api-dvb-nit-settings
source_filename: medialive-api-dvb-nit-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-nit-settings-schema.json\",\n  \"title\": \"DvbNitSettings\",\n  \"description\": \"DVB Network Information Table (NIT)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65536\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkId\"\n          },\n          \"description\": \"The numeric value placed in the Network Information Table (NIT).\"\n        }\n      ]\n    },\n    \"NetworkName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkName\"\n          },\n          \"description\": \"The network name text placed in the\
  \ networkNameDescriptor inside the Network Information Table. Maximum length is 256 characters.\"\n        }\n      ]\n    },\n    \"RepInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin25Max10000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"repInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NetworkName\",\n    \"NetworkId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-nit-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DvbNitSettings
---
