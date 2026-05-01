---
description: Nielsen Configuration
layout: schema
name: NielsenConfiguration
properties_list:
- description: ''
  name: DistributorId
  type: object
- description: ''
  name: NielsenPcmToId3Tagging
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-nielsen-configuration-schema.json
slug: medialive-api-nielsen-configuration
source_filename: medialive-api-nielsen-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-configuration-schema.json\",\n  \"title\": \"NielsenConfiguration\",\n  \"description\": \"Nielsen Configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DistributorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"distributorId\"\n          },\n          \"description\": \"Enter the Distributor ID assigned to your organization by Nielsen.\"\n        }\n      ]\n    },\n    \"NielsenPcmToId3Tagging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenPcmToId3TaggingState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenPcmToId3Tagging\"\n          },\n          \"description\": \"Enables Nielsen\
  \ PCM to ID3 tagging\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-nielsen-configuration-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NielsenConfiguration
---
