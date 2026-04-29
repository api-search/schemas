---
description: Placeholder documentation for ChannelEgressEndpoint
layout: schema
name: ChannelEgressEndpoint
properties_list:
- description: ''
  name: SourceIp
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-channel-egress-endpoint-schema.json
slug: medialive-api-channel-egress-endpoint
source_filename: medialive-api-channel-egress-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-channel-egress-endpoint-schema.json\",\n  \"title\": \"ChannelEgressEndpoint\",\n  \"description\": \"Placeholder documentation for ChannelEgressEndpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceIp\"\n          },\n          \"description\": \"Public IP of where a channel's output comes from\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-channel-egress-endpoint-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ChannelEgressEndpoint
---
