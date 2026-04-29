---
description: ListQueuesResponse schema from Amazon MediaConvert API
layout: schema
name: ListQueuesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Queues
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-list-queues-response-schema.json
slug: mediaconvert-api-list-queues-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-queues-response-schema.json\",\n  \"title\": \"ListQueuesResponse\",\n  \"description\": \"ListQueuesResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Use this string to request the next batch of queues.\"\n        }\n      ]\n    },\n    \"Queues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfQueue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queues\"\n          },\n          \"description\": \"List of queues.\"\n        }\n      ]\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-list-queues-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListQueuesResponse
---
