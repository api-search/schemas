---
description: Placeholder documentation for ListChannelsResponse
layout: schema
name: ListChannelsResponse
properties_list:
- description: ''
  name: Channels
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-channels-response-schema.json
slug: medialive-api-list-channels-response
source_filename: medialive-api-list-channels-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-channels-response-schema.json\",\n  \"title\": \"ListChannelsResponse\",\n  \"description\": \"Placeholder documentation for ListChannelsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfChannelSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\n          }\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-channels-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListChannelsResponse
---
