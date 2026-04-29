---
description: ConversationAnalytics from WhatsApp API
layout: schema
name: ConversationAnalytics
properties_list:
- description: ''
  name: conversation_analytics
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-conversation-analytics-schema.json
slug: whatsapp-business-management-api-conversation-analytics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-conversation-analytics-schema.json\",\n  \"title\": \"ConversationAnalytics\",\n  \"description\": \"ConversationAnalytics from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conversation_analytics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"data_points\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"start\": {\n                      \"type\": \"integer\"\n                    },\n                    \"end\": {\n                      \"type\": \"integer\"\n   \
  \                 },\n                    \"conversation\": {\n                      \"type\": \"integer\"\n                    },\n                    \"cost\": {\n                      \"type\": \"number\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-conversation-analytics-schema.json
tags: []
title: ConversationAnalytics
---
