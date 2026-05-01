---
description: An event card archived in the Global Relay Archive, representing activity from collaboration platforms, social media, or customer experience tools. Cards contain sections, each with individual events.
layout: schema
name: Global Relay Event Card
properties_list:
- description: Unique identifier for the event card
  name: cardId
  type: string
- description: The type of digital channel
  name: channelType
  type: string
- description: Title of the event card
  name: title
  type: string
- description: Source platform name
  name: source
  type: string
- description: Sections within the event card
  name: sections
  type: array
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-event-card.json
slug: global-relay-event-card
source_filename: global-relay-event-card.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-event-card.json\",\n  \"title\": \"Global Relay Event Card\",\n  \"description\": \"An event card archived in the Global Relay Archive, representing activity from collaboration platforms, social media, or customer experience tools. Cards contain sections, each with individual events.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"cardId\",\n    \"channelType\",\n    \"sections\"\n  ],\n  \"properties\": {\n    \"cardId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event card\"\n    },\n    \"channelType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of digital channel\",\n      \"enum\": [\n        \"SocialMedia\",\n        \"Collaboration\",\n        \"CustomerExperience\",\n        \"Website\",\n        \"Other\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of\
  \ the event card\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source platform name\"\n    },\n    \"sections\": {\n      \"type\": \"array\",\n      \"description\": \"Sections within the event card\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"sectionId\",\n          \"events\"\n        ],\n        \"properties\": {\n          \"sectionId\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the section\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"Title of the section\"\n          },\n          \"events\": {\n            \"type\": \"array\",\n            \"description\": \"Events within this section\",\n            \"items\": {\n              \"type\": \"object\",\n              \"required\": [\n                \"eventType\",\n                \"timestamp\"\n              ],\n              \"properties\"\
  : {\n                \"eventType\": {\n                  \"type\": \"string\",\n                  \"description\": \"Type of event\",\n                  \"enum\": [\n                    \"Post\",\n                    \"Comment\",\n                    \"Reply\",\n                    \"Reaction\",\n                    \"Share\",\n                    \"Edit\",\n                    \"Delete\",\n                    \"Like\",\n                    \"Follow\"\n                  ]\n                },\n                \"timestamp\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\",\n                  \"description\": \"Timestamp of the event in ISO 8601 format\"\n                },\n                \"author\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"authorId\": {\n                      \"type\": \"string\",\n                      \"description\": \"Unique identifier for the author\"\n          \
  \          },\n                    \"displayName\": {\n                      \"type\": \"string\",\n                      \"description\": \"Display name of the author\"\n                    },\n                    \"email\": {\n                      \"type\": \"string\",\n                      \"format\": \"email\",\n                      \"description\": \"Email address of the author\"\n                    }\n                  }\n                },\n                \"body\": {\n                  \"type\": \"string\",\n                  \"description\": \"Content body of the event\"\n                },\n                \"fileIds\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  },\n                  \"description\": \"IDs of files uploaded via /files endpoint\"\n                },\n                \"metadata\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\":\
  \ {\n                    \"type\": \"string\"\n                  },\n                  \"description\": \"Additional metadata key-value pairs\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-event-card.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Event Card
---
