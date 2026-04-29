---
description: Configuration parameters used to update the Channel.
layout: schema
name: UpdateChannelRequest
properties_list:
- description: ''
  name: Description
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-update-channel-request-schema.json
slug: mediapackage-api-update-channel-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-update-channel-request-schema.json\",\n  \"title\": \"UpdateChannelRequest\",\n  \"description\": \"Configuration parameters used to update the Channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A short text description of the Channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-update-channel-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateChannelRequest
---
