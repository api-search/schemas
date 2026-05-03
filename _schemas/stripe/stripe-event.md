---
description: Events are Stripe's way of letting you know when something interesting happens in your account. When an interesting event occurs, a new Event object is created and POSTed to the configured webhook URL.
layout: schema
name: Stripe Event
properties_list:
- description: Unique identifier for the object.
  name: id
  type: string
- description: String representing the object's type.
  name: object
  type: string
- description: The connected account that originated the event.
  name: account
  type: string
- description: The Stripe API version used to render data.
  name: api_version
  type:
  - string
  - 'null'
- description: Time at which the object was created. Measured in seconds since the Unix epoch.
  name: created
  type: integer
- description: Object containing data associated with the event.
  name: data
  type: object
- description: Has the value true if the object exists in live mode or the value false if the object exists in test mode.
  name: livemode
  type: boolean
- description: Number of webhooks that haven't been successfully delivered (i.e., to return a 20x response) to the URLs you specify.
  name: pending_webhooks
  type: integer
- description: Information on the API request that triggers the event.
  name: request
  type:
  - object
  - 'null'
- description: Description of the event (e.g., invoice.created or charge.refunded).
  name: type
  type: string
provider_name: Stripe
provider_slug: stripe
schema_file: json-schema/stripe-event.json
slug: stripe-event
source_filename: stripe-event.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stripe.com/schemas/event\",\n  \"title\": \"Stripe Event\",\n  \"description\": \"Events are Stripe's way of letting you know when something interesting happens in your account. When an interesting event occurs, a new Event object is created and POSTed to the configured webhook URL.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the object.\",\n      \"pattern\": \"^evt_\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"event\",\n      \"description\": \"String representing the object's type.\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"The connected account that originated the event.\"\n    },\n    \"api_version\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Stripe API version used to render data.\"\
  \n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the object was created. Measured in seconds since the Unix epoch.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Object containing data associated with the event.\",\n      \"properties\": {\n        \"object\": {\n          \"type\": \"object\",\n          \"description\": \"Object containing the API resource relevant to the event.\"\n        },\n        \"previous_attributes\": {\n          \"type\": \"object\",\n          \"description\": \"Object containing the names of the updated attributes and their values prior to the event (only included in *.updated events).\"\n        }\n      },\n      \"required\": [\"object\"]\n    },\n    \"livemode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Has the value true if the object exists in live mode or the value false if the object exists in test mode.\"\n    },\n    \"pending_webhooks\": {\n \
  \     \"type\": \"integer\",\n      \"description\": \"Number of webhooks that haven't been successfully delivered (i.e., to return a 20x response) to the URLs you specify.\"\n    },\n    \"request\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Information on the API request that triggers the event.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"ID of the API request that caused the event.\"\n        },\n        \"idempotency_key\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The idempotency key transmitted during the request, if any.\"\n        }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the event (e.g., invoice.created or charge.refunded).\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"object\",\n    \"api_version\",\n    \"created\",\n    \"data\",\n    \"livemode\",\n    \"pending_webhooks\"\
  ,\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stripe/refs/heads/main/json-schema/stripe-event.json
tags:
- Commerce
- Financial Services
- Fintech
- Payments
- T1
title: Stripe Event
---
