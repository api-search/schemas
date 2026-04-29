---
description: Delivery made by a webhook.
layout: schema
name: hook-delivery
properties_list:
- description: Unique identifier of the delivery.
  name: id
  type: integer
- description: Unique identifier for the event (shared with all deliveries for all webhooks that subscribe to this event).
  name: guid
  type: string
- description: Time when the delivery was delivered.
  name: delivered_at
  type: string
- description: Whether the delivery is a redelivery.
  name: redelivery
  type: boolean
- description: Time spent delivering.
  name: duration
  type: number
- description: Description of the status of the attempted delivery
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
- description: The URL target of the delivery.
  name: url
  type: string
- description: ''
  name: request
  type: object
- description: ''
  name: response
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-app-api-hook-delivery-schema.json
slug: github-app-api-hook-delivery
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-hook-delivery-schema.json\",\n  \"title\": \"hook-delivery\",\n  \"description\": \"Delivery made by a webhook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the delivery.\",\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"guid\": {\n      \"description\": \"Unique identifier for the event (shared with all deliveries for all webhooks that subscribe to this event).\",\n      \"type\": \"string\",\n      \"example\": \"58474f00-b361-11eb-836d-0e4f3503ccbe\"\n    },\n    \"delivered_at\": {\n      \"description\": \"Time when the delivery was delivered.\",\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-05-12T20:33:44Z\"\n    },\n    \"redelivery\": {\n      \"description\"\
  : \"Whether the delivery is a redelivery.\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"duration\": {\n      \"description\": \"Time spent delivering.\",\n      \"type\": \"number\",\n      \"example\": 0.03\n    },\n    \"status\": {\n      \"description\": \"Description of the status of the attempted delivery\",\n      \"type\": \"string\",\n      \"example\": \"failed to connect\"\n    },\n    \"status_code\": {\n      \"description\": \"Status code received when delivery was made.\",\n      \"type\": \"integer\",\n      \"example\": 502\n    },\n    \"event\": {\n      \"description\": \"The event that triggered the delivery.\",\n      \"type\": \"string\",\n      \"example\": \"issues\"\n    },\n    \"action\": {\n      \"description\": \"The type of activity for the event that triggered the delivery.\",\n      \"type\": \"string\",\n      \"example\": \"opened\",\n      \"nullable\": true\n    },\n    \"installation_id\": {\n      \"description\": \"The\
  \ id of the GitHub App installation associated with this event.\",\n      \"type\": \"integer\",\n      \"example\": 123,\n      \"nullable\": true\n    },\n    \"repository_id\": {\n      \"description\": \"The id of the repository associated with this event.\",\n      \"type\": \"integer\",\n      \"example\": 123,\n      \"nullable\": true\n    },\n    \"url\": {\n      \"description\": \"The URL target of the delivery.\",\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"request\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"headers\": {\n          \"description\": \"The request headers sent with the webhook delivery.\",\n          \"type\": \"object\",\n          \"nullable\": true,\n          \"additionalProperties\": true\n        },\n        \"payload\": {\n          \"description\": \"The webhook payload.\",\n          \"type\": \"object\",\n          \"nullable\": true,\n          \"additionalProperties\": true\n\
  \        }\n      },\n      \"required\": [\n        \"headers\",\n        \"payload\"\n      ]\n    },\n    \"response\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"headers\": {\n          \"description\": \"The response headers received when the delivery was made.\",\n          \"type\": \"object\",\n          \"nullable\": true,\n          \"additionalProperties\": true\n        },\n        \"payload\": {\n          \"description\": \"The response payload received.\",\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"additionalProperties\": true\n        }\n      },\n      \"required\": [\n        \"headers\",\n        \"payload\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"guid\",\n    \"delivered_at\",\n    \"redelivery\",\n    \"duration\",\n    \"status\",\n    \"status_code\",\n    \"event\",\n    \"action\",\n    \"installation_id\",\n    \"repository_id\",\n    \"request\",\n    \"response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-hook-delivery-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: hook-delivery
---
