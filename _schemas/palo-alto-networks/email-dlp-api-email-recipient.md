---
description: EmailRecipient schema from Palo Alto Networks Email DLP API
layout: schema
name: EmailRecipient
properties_list:
- description: Recipient email address.
  name: email
  type: string
- description: Recipient type indicating address field.
  name: type
  type: string
- description: Delivery status of the message to this recipient.
  name: delivery_status
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/email-dlp-api-email-recipient-schema.json
slug: email-dlp-api-email-recipient
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailRecipient\",\n  \"description\": \"EmailRecipient schema from Palo Alto Networks Email DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/email-dlp-api-email-recipient-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient email address.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"to\",\n        \"cc\",\n        \"bcc\"\n      ],\n      \"description\": \"Recipient type indicating address field.\"\n    },\n    \"delivery_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"delivered\",\n        \"blocked\",\n        \"quarantined\",\n        \"pending\"\n      ],\n      \"description\": \"Delivery status of the message to this recipient.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/email-dlp-api-email-recipient-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailRecipient
---
