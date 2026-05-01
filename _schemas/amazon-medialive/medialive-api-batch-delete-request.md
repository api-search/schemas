---
description: A request to delete resources
layout: schema
name: BatchDeleteRequest
properties_list:
- description: ''
  name: ChannelIds
  type: object
- description: ''
  name: InputIds
  type: object
- description: ''
  name: InputSecurityGroupIds
  type: object
- description: ''
  name: MultiplexIds
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-batch-delete-request-schema.json
slug: medialive-api-batch-delete-request
source_filename: medialive-api-batch-delete-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-delete-request-schema.json\",\n  \"title\": \"BatchDeleteRequest\",\n  \"description\": \"A request to delete resources\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelIds\"\n          },\n          \"description\": \"List of channel IDs\"\n        }\n      ]\n    },\n    \"InputIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputIds\"\n          },\n          \"description\": \"List of input IDs\"\n        }\n      ]\n    },\n    \"InputSecurityGroupIds\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSecurityGroupIds\"\n          },\n          \"description\": \"List of input security group IDs\"\n        }\n      ]\n    },\n    \"MultiplexIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexIds\"\n          },\n          \"description\": \"List of multiplex IDs\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-batch-delete-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BatchDeleteRequest
---
