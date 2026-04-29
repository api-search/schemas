---
description: Represents a webhook event payload delivered by Brevo when an email interaction occurs, including delivery status changes, opens, clicks, bounces, and spam reports.
layout: schema
name: Brevo Email Event
properties_list:
- description: Type of email event that occurred.
  name: event
  type: string
- description: Recipient email address associated with the event.
  name: email
  type: string
- description: Internal Brevo event identifier.
  name: id
  type: integer
- description: UTC date-time when the event occurred.
  name: date
  type: string
- description: Unique identifier of the email message that triggered the event.
  name: messageId
  type: string
- description: Subject line of the email message.
  name: subject
  type: string
- description: Tag assigned to the email for categorization and tracking.
  name: tag
  type: string
- description: IP address of the server used to send the email.
  name: sendingIp
  type: string
- description: Unix timestamp in seconds when the event occurred.
  name: ts
  type: integer
- description: Unix timestamp in milliseconds when the event occurred.
  name: ts_epoch
  type: integer
- description: Reason for the event if applicable, such as bounce error codes or spam filter details.
  name: reason
  type: string
- description: URL of the link that was clicked, present only for click events.
  name: link
  type: string
- description: ID of the template used for the email if applicable.
  name: templateId
  type: integer
- description: ID of the marketing campaign if the event is for a campaign email.
  name: campaignId
  type: integer
provider_name: brevo
provider_slug: brevo
schema_file: json-schema/brevo-email-event-schema.json
slug: brevo-email-event
source_filename: brevo-email-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://brevo.com/schemas/brevo/email-event.json\",\n  \"title\": \"Brevo Email Event\",\n  \"description\": \"Represents a webhook event payload delivered by Brevo when an email interaction occurs, including delivery status changes, opens, clicks, bounces, and spam reports.\",\n  \"type\": \"object\",\n  \"required\": [\"event\", \"email\", \"date\"],\n  \"properties\": {\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Type of email event that occurred.\",\n      \"enum\": [\n        \"sent\",\n        \"request\",\n        \"delivered\",\n        \"hardBounce\",\n        \"softBounce\",\n        \"blocked\",\n        \"spam\",\n        \"invalid\",\n        \"deferred\",\n        \"opened\",\n        \"uniqueOpened\",\n        \"clicked\",\n        \"unsubscribed\",\n        \"proxyOpen\",\n        \"uniqueProxyOpen\"\n      ]\n    },\n    \"email\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"email\",\n      \"description\": \"Recipient email address associated with the event.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal Brevo event identifier.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC date-time when the event occurred.\"\n    },\n    \"messageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the email message that triggered the event.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Subject line of the email message.\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Tag assigned to the email for categorization and tracking.\"\n    },\n    \"sendingIp\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IP address of the server used to send the email.\"\n    },\n    \"ts\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"Unix timestamp in seconds when the event occurred.\"\n    },\n    \"ts_epoch\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the event occurred.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the event if applicable, such as bounce error codes or spam filter details.\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the link that was clicked, present only for click events.\"\n    },\n    \"templateId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the template used for the email if applicable.\"\n    },\n    \"campaignId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the marketing campaign if the event is for a campaign email.\"\n    }\n  },\n  \"$defs\": {\n    \"TransactionalEmailEvent\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Event payload specific to transactional email events.\",\n      \"allOf\": [\n        { \"$ref\": \"#\" },\n        {\n          \"properties\": {\n            \"event\": {\n              \"enum\": [\n                \"sent\",\n                \"request\",\n                \"delivered\",\n                \"hardBounce\",\n                \"softBounce\",\n                \"blocked\",\n                \"spam\",\n                \"invalid\",\n                \"deferred\",\n                \"opened\",\n                \"uniqueOpened\",\n                \"clicked\",\n                \"unsubscribed\"\n              ]\n            }\n          }\n        }\n      ]\n    },\n    \"MarketingEmailEvent\": {\n      \"type\": \"object\",\n      \"description\": \"Event payload specific to marketing campaign email events.\",\n      \"allOf\": [\n        { \"$ref\": \"#\" },\n        {\n          \"properties\": {\n            \"event\": {\n              \"enum\": [\n                \"delivered\"\
  ,\n                \"opened\",\n                \"clicked\",\n                \"hardBounce\",\n                \"softBounce\",\n                \"spam\",\n                \"unsubscribed\",\n                \"proxyOpen\"\n              ]\n            }\n          },\n          \"required\": [\"campaignId\"]\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/json-schema/brevo-email-event-schema.json
tags: []
title: Brevo Email Event
---
