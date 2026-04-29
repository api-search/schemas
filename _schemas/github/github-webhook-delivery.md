---
description: A record of a webhook delivery from GitHub, including the request headers, payload, and response information.
layout: schema
name: GitHub Webhook Delivery
properties_list:
- description: The unique identifier of the webhook delivery.
  name: id
  type: integer
- description: The globally unique identifier for the delivery (X-GitHub-Delivery header).
  name: guid
  type: string
- description: The date and time the delivery was made.
  name: delivered_at
  type: string
- description: Whether this delivery is a redelivery of a previous delivery.
  name: redelivery
  type: boolean
- description: The time in seconds the delivery took.
  name: duration
  type: number
- description: The HTTP status description returned by the receiver.
  name: status
  type: string
- description: The HTTP status code returned by the receiver.
  name: status_code
  type: integer
- description: The event type that triggered the delivery (X-GitHub-Event header).
  name: event
  type: string
- description: The action within the event that triggered the delivery.
  name: action
  type:
  - string
  - 'null'
- description: The GitHub App installation ID, if applicable.
  name: installation_id
  type:
  - integer
  - 'null'
- description: The repository ID associated with the delivery.
  name: repository_id
  type:
  - integer
  - 'null'
- description: The API URL for the delivery record.
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
schema_file: json-schema/github-webhook-delivery-schema.json
slug: github-webhook-delivery
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/schemas/github/webhook-delivery.json\",\n  \"title\": \"GitHub Webhook Delivery\",\n  \"description\": \"A record of a webhook delivery from GitHub, including the request headers, payload, and response information.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"guid\", \"event\", \"action\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the webhook delivery.\"\n    },\n    \"guid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The globally unique identifier for the delivery (X-GitHub-Delivery header).\"\n    },\n    \"delivered_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the delivery was made.\"\n    },\n    \"redelivery\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ this delivery is a redelivery of a previous delivery.\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"The time in seconds the delivery took.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP status description returned by the receiver.\"\n    },\n    \"status_code\": {\n      \"type\": \"integer\",\n      \"minimum\": 100,\n      \"maximum\": 599,\n      \"description\": \"The HTTP status code returned by the receiver.\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"The event type that triggered the delivery (X-GitHub-Event header).\"\n    },\n    \"action\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The action within the event that triggered the delivery.\"\n    },\n    \"installation_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The GitHub App installation ID, if applicable.\"\n    },\n  \
  \  \"repository_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The repository ID associated with the delivery.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the delivery record.\"\n    },\n    \"request\": {\n      \"$ref\": \"#/$defs/DeliveryRequest\"\n    },\n    \"response\": {\n      \"$ref\": \"#/$defs/DeliveryResponse\"\n    }\n  },\n  \"$defs\": {\n    \"DeliveryRequest\": {\n      \"type\": \"object\",\n      \"description\": \"The HTTP request that was sent to the webhook receiver.\",\n      \"properties\": {\n        \"headers\": {\n          \"type\": \"object\",\n          \"description\": \"The HTTP headers sent with the request.\",\n          \"properties\": {\n            \"X-GitHub-Hook-ID\": {\n              \"type\": \"string\",\n              \"description\": \"Unique identifier for the webhook configuration.\"\n            },\n            \"X-GitHub-Event\": {\n\
  \              \"type\": \"string\",\n              \"description\": \"The name of the event that triggered the delivery.\"\n            },\n            \"X-GitHub-Delivery\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\",\n              \"description\": \"A GUID to uniquely identify the delivery.\"\n            },\n            \"X-Hub-Signature-256\": {\n              \"type\": \"string\",\n              \"pattern\": \"^sha256=[0-9a-f]{64}$\",\n              \"description\": \"HMAC-SHA256 hex digest of the payload, prefixed with sha256=.\"\n            },\n            \"X-Hub-Signature\": {\n              \"type\": \"string\",\n              \"pattern\": \"^sha1=[0-9a-f]{40}$\",\n              \"description\": \"Legacy HMAC-SHA1 hex digest of the payload, prefixed with sha1=.\"\n            },\n            \"X-GitHub-Hook-Installation-Target-Type\": {\n              \"type\": \"string\",\n              \"enum\": [\"repository\", \"organization\", \"business\"\
  , \"app\"],\n              \"description\": \"The type of resource the webhook is installed on.\"\n            },\n            \"X-GitHub-Hook-Installation-Target-ID\": {\n              \"type\": \"string\",\n              \"description\": \"The unique identifier of the resource the webhook is installed on.\"\n            },\n            \"User-Agent\": {\n              \"type\": \"string\",\n              \"pattern\": \"^GitHub-Hookshot/\",\n              \"description\": \"The GitHub user agent string.\"\n            },\n            \"Content-Type\": {\n              \"type\": \"string\",\n              \"enum\": [\"application/json\", \"application/x-www-form-urlencoded\"],\n              \"description\": \"The content type of the payload.\"\n            }\n          }\n        },\n        \"payload\": {\n          \"type\": \"object\",\n          \"description\": \"The JSON payload that was sent.\"\n        }\n      }\n    },\n    \"DeliveryResponse\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"The HTTP response received from the webhook receiver.\",\n      \"properties\": {\n        \"headers\": {\n          \"type\": \"object\",\n          \"description\": \"The HTTP response headers.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"payload\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The response body returned by the receiver.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-webhook-delivery-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: GitHub Webhook Delivery
---
