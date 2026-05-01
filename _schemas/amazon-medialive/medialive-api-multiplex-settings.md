---
description: Contains configuration for a Multiplex event
layout: schema
name: MultiplexSettings
properties_list:
- description: ''
  name: MaximumVideoBufferDelayMilliseconds
  type: object
- description: ''
  name: TransportStreamBitrate
  type: object
- description: ''
  name: TransportStreamId
  type: object
- description: ''
  name: TransportStreamReservedBitrate
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-settings-schema.json
slug: medialive-api-multiplex-settings
source_filename: medialive-api-multiplex-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-settings-schema.json\",\n  \"title\": \"MultiplexSettings\",\n  \"description\": \"Contains configuration for a Multiplex event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaximumVideoBufferDelayMilliseconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin800Max3000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumVideoBufferDelayMilliseconds\"\n          },\n          \"description\": \"Maximum video buffer delay in milliseconds.\"\n        }\n      ]\n    },\n    \"TransportStreamBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1000000Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamBitrate\"\
  \n          },\n          \"description\": \"Transport stream bit rate.\"\n        }\n      ]\n    },\n    \"TransportStreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamId\"\n          },\n          \"description\": \"Transport stream ID.\"\n        }\n      ]\n    },\n    \"TransportStreamReservedBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamReservedBitrate\"\n          },\n          \"description\": \"Transport stream reserved bit rate.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TransportStreamBitrate\",\n    \"TransportStreamId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MultiplexSettings
---
