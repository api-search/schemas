---
description: A new Channel configuration.
layout: schema
name: CreateChannelRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-create-channel-request-schema.json
slug: mediapackage-api-create-channel-request
source_filename: mediapackage-api-create-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-create-channel-request-schema.json\",\n  \"title\": \"CreateChannelRequest\",\n  \"description\": \"A new Channel configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A short text description of the Channel.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The ID of the Channel. The ID must be unique within the region and it\\ncannot be changed\
  \ after a Channel is created.\\n\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-create-channel-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateChannelRequest
---
