---
description: Delivery made by a webhook, without request and response information.
layout: schema
name: hook-delivery-item
properties_list:
- description: Unique identifier of the webhook delivery.
  name: id
  type: integer
- description: Unique identifier for the event (shared with all deliveries for all webhooks that subscribe to this event).
  name: guid
  type: string
- description: Time when the webhook delivery occurred.
  name: delivered_at
  type: string
- description: Whether the webhook delivery is a redelivery.
  name: redelivery
  type: boolean
- description: Time spent delivering.
  name: duration
  type: number
- description: Describes the response returned after attempting the delivery.
  name: status
  type: string
- description: Status code received when delivery was made.
  name: status_code
  type: integer
- description: The event that triggered the delivery.
  name: event
  type: string
- description: The type of activity for the event that triggered the delivery.
  name: action
  type: string
- description: The id of the GitHub App installation associated with this event.
  name: installation_id
  type: integer
- description: The id of the repository associated with this event.
  name: repository_id
  type: integer
- description: Time when the webhook delivery was throttled.
  name: throttled_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-hooks-api-hook-delivery-item-schema.json
slug: github-repo-hooks-api-hook-delivery-item
source_filename: github-repo-hooks-api-hook-delivery-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-hooks-api-hook-delivery-item-schema.json\",\n  \"title\": \"hook-delivery-item\",\n  \"description\": \"Delivery made by a webhook, without request and response information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the webhook delivery.\",\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"guid\": {\n      \"description\": \"Unique identifier for the event (shared with all deliveries for all webhooks that subscribe to this event).\",\n      \"type\": \"string\",\n      \"example\": \"58474f00-b361-11eb-836d-0e4f3503ccbe\"\n    },\n    \"delivered_at\": {\n      \"description\": \"Time when the webhook delivery occurred.\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-05-12T20:33:44Z\"\
  \n    },\n    \"redelivery\": {\n      \"description\": \"Whether the webhook delivery is a redelivery.\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"duration\": {\n      \"description\": \"Time spent delivering.\",\n      \"type\": \"number\",\n      \"example\": 0.03\n    },\n    \"status\": {\n      \"description\": \"Describes the response returned after attempting the delivery.\",\n      \"type\": \"string\",\n      \"example\": \"failed to connect\"\n    },\n    \"status_code\": {\n      \"description\": \"Status code received when delivery was made.\",\n      \"type\": \"integer\",\n      \"example\": 502\n    },\n    \"event\": {\n      \"description\": \"The event that triggered the delivery.\",\n      \"type\": \"string\",\n      \"example\": \"issues\"\n    },\n    \"action\": {\n      \"description\": \"The type of activity for the event that triggered the delivery.\",\n      \"type\": \"string\",\n      \"example\": \"opened\"\n    },\n    \"installation_id\"\
  : {\n      \"description\": \"The id of the GitHub App installation associated with this event.\",\n      \"type\": \"integer\",\n      \"example\": 123\n    },\n    \"repository_id\": {\n      \"description\": \"The id of the repository associated with this event.\",\n      \"type\": \"integer\",\n      \"example\": 123\n    },\n    \"throttled_at\": {\n      \"description\": \"Time when the webhook delivery was throttled.\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-05-12T20:33:44Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"guid\",\n    \"delivered_at\",\n    \"redelivery\",\n    \"duration\",\n    \"status\",\n    \"status_code\",\n    \"event\",\n    \"action\",\n    \"installation_id\",\n    \"repository_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-hooks-api-hook-delivery-item-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: hook-delivery-item
---
