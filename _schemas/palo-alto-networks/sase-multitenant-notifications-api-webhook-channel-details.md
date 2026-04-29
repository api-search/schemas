---
description: WebhookChannelDetails schema from Multi-Tenant Notifications API
layout: schema
name: WebhookChannelDetails
properties_list:
- description: List of Webhook URLs - do not include token in the URL
  name: urls
  type: array
- description: Webhook Authentication Type
  name: authType
  type: string
- description: Webhook token value
  name: token
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-webhook-channel-details-schema.json
slug: sase-multitenant-notifications-api-webhook-channel-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebhookChannelDetails\",\n  \"description\": \"WebhookChannelDetails schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-webhook-channel-details-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"urls\": {\n      \"description\": \"List of Webhook URLs - do not include token in the URL\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"authType\": {\n      \"description\": \"Webhook Authentication Type\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"NO_AUTH\",\n        \"TOKEN\"\n      ]\n    },\n    \"token\": {\n      \"description\": \"Webhook token value\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"urls\",\n    \"authType\",\n    \"token\"\n \
  \ ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-webhook-channel-details-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: WebhookChannelDetails
---
