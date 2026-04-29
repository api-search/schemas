---
description: EmailChannelDetails schema from Multi-Tenant Notifications API
layout: schema
name: EmailChannelDetails
properties_list:
- description: List of emails
  name: emails
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-email-channel-details-schema.json
slug: sase-multitenant-notifications-api-email-channel-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailChannelDetails\",\n  \"description\": \"EmailChannelDetails schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-email-channel-details-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"emails\": {\n      \"description\": \"List of emails\",\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"name\",\n          \"emailId\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"description\": \"Email owner name\",\n            \"type\": \"string\"\n          },\n          \"emailId\": {\n            \"description\": \"Email id\",\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"emails\"\n  ]\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-email-channel-details-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailChannelDetails
---
