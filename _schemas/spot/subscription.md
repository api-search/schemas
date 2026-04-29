---
description: A Spot subscription defines an event notification configuration, delivering alerts about Spot resource events to a specified endpoint via a chosen protocol.
layout: schema
name: Spot Subscription
properties_list:
- description: The unique identifier of the subscription.
  name: id
  type: string
- description: The identifier of the resource to monitor.
  name: resourceId
  type: string
- description: The protocol used to deliver event notifications.
  name: protocol
  type: string
- description: The endpoint URL or address where notifications are sent.
  name: endpoint
  type: string
- description: The type of event to subscribe to.
  name: eventType
  type: string
- description: Custom formatting options for the event notification payload.
  name: eventFormat
  type: object
provider_name: Spot
provider_slug: spot
schema_file: json-schema/subscription.json
slug: subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/subscription.json\",\n  \"title\": \"Spot Subscription\",\n  \"description\": \"A Spot subscription defines an event notification configuration, delivering alerts about Spot resource events to a specified endpoint via a chosen protocol.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the subscription.\"\n    },\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the resource to monitor.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"enum\": [\"http\", \"https\", \"email\", \"email-json\", \"aws-sns\", \"web\"],\n      \"description\": \"The protocol used to deliver event notifications.\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ endpoint URL or address where notifications are sent.\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event to subscribe to.\"\n    },\n    \"eventFormat\": {\n      \"type\": \"object\",\n      \"description\": \"Custom formatting options for the event notification payload.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/subscription.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Subscription
---
