---
description: The Chatbot chat channel used for collaboration during an incident.
layout: schema
name: ChatChannel
properties_list:
- description: ''
  name: chatbotSns
  type: object
- description: ''
  name: empty
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-chat-channel-schema.json
slug: incident-manager-chat-channel
source_filename: incident-manager-chat-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-chat-channel-schema.json\",\n  \"title\": \"ChatChannel\",\n  \"description\": \"The Chatbot chat channel used for collaboration during an incident.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chatbotSns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChatbotSnsConfigurationSet\"\n        },\n        {\n          \"description\": \"The Amazon SNS targets that Chatbot uses to notify the chat channel of updates to an incident. You can also make updates to the incident through the chat channel by using the Amazon SNS topics. \"\n        }\n      ]\n    },\n    \"empty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyChatChannel\"\n        },\n        {\n          \"description\": \"Used to remove the chat\
  \ channel from an incident record or response plan.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-chat-channel-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: ChatChannel
---
