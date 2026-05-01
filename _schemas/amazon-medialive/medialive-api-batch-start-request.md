---
description: A request to start resources
layout: schema
name: BatchStartRequest
properties_list:
- description: ''
  name: ChannelIds
  type: object
- description: ''
  name: MultiplexIds
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-start-request-schema.json
slug: medialive-api-batch-start-request
source_filename: medialive-api-batch-start-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-start-request-schema.json\",\n  \"title\": \"BatchStartRequest\",\n  \"description\": \"A request to start resources\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelIds\"\n          },\n          \"description\": \"List of channel IDs\"\n        }\n      ]\n    },\n    \"MultiplexIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexIds\"\n          },\n          \"description\": \"List of multiplex IDs\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-start-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BatchStartRequest
---
