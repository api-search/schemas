---
description: Contains summary configuration for a Multiplex event.
layout: schema
name: MultiplexSettingsSummary
properties_list:
- description: ''
  name: TransportStreamBitrate
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-settings-summary-schema.json
slug: medialive-api-multiplex-settings-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-settings-summary-schema.json\",\n  \"title\": \"MultiplexSettingsSummary\",\n  \"description\": \"Contains summary configuration for a Multiplex event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransportStreamBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000000Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamBitrate\"\n          },\n          \"description\": \"Transport stream bit rate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-settings-summary-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexSettingsSummary
---
