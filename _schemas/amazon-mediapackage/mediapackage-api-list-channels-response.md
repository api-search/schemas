---
description: ListChannelsResponse schema from Amazon MediaPackage API
layout: schema
name: ListChannelsResponse
properties_list:
- description: ''
  name: Channels
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-list-channels-response-schema.json
slug: mediapackage-api-list-channels-response
source_filename: mediapackage-api-list-channels-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-list-channels-response-schema.json\",\n  \"title\": \"ListChannelsResponse\",\n  \"description\": \"ListChannelsResponse schema from Amazon MediaPackage API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfChannel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channels\"\n          },\n          \"description\": \"A list of Channel records.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"A token that can be used to resume pagination from the end\
  \ of the collection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-list-channels-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListChannelsResponse
---
