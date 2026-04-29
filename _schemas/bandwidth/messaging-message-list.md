---
description: MessageList schema from Bandwidth messaging API
layout: schema
name: MessageList
properties_list:
- description: The total number of messages matching the query
  name: totalCount
  type: integer
- description: ''
  name: pageInfo
  type: object
- description: ''
  name: messages
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-message-list-schema.json
slug: messaging-message-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-message-list-schema.json\",\n  \"title\": \"MessageList\",\n  \"description\": \"MessageList schema from Bandwidth messaging API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of messages matching the query\"\n    },\n    \"pageInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prevPage\": {\n          \"type\": \"string\",\n          \"description\": \"Token for the previous page\"\n        },\n        \"nextPage\": {\n          \"type\": \"string\",\n          \"description\": \"Token for the next page\"\n        },\n        \"prevPageToken\": {\n          \"type\": \"string\",\n          \"description\": \"Previous page token for pagination\"\n        },\n        \"nextPageToken\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Next page token for pagination\"\n        }\n      }\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Message\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-message-list-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: MessageList
---
