---
description: An event action that automates responses to Data Exchange events.
layout: schema
name: Event Action
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: Event
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/event-action-schema.json
slug: event-action
source_filename: event-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/event-action-schema.json\",\n  \"title\": \"Event Action\",\n  \"description\": \"An event action that automates responses to Data Exchange events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"Event\": {\n      \"type\": \"object\"\n    },\n    \"Action\": {\n      \"type\": \"object\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/event-action-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Event Action
---
