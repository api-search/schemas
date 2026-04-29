---
description: NotifChannel schema from Multi-Tenant Notifications API
layout: schema
name: NotifChannel
properties_list:
- description: Notification channel name
  name: name
  type: string
- description: Notification channel type
  name: type
  type: string
- description: Email channel details
  name: emailChannelDetails
  type: object
- description: Webhook channel details
  name: webhookChannelDetails
  type: object
- description: Channel output template
  name: template
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-channel-schema.json
slug: sase-multitenant-notifications-api-notif-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifChannel\",\n  \"description\": \"NotifChannel schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-channel-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Notification channel name\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Notification channel type\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"EMAIL\",\n        \"WEBHOOK\"\n      ]\n    },\n    \"emailChannelDetails\": {\n      \"description\": \"Email channel details\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"required\": [\n          \"emails\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"emails\": {\n          \
  \  \"description\": \"List of emails\",\n            \"type\": \"array\",\n            \"items\": {\n              \"required\": [\n                \"name\",\n                \"emailId\"\n              ],\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"description\": \"Email owner name\",\n                  \"type\": \"string\"\n                },\n                \"emailId\": {\n                  \"description\": \"Email id\",\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"webhookChannelDetails\": {\n      \"description\": \"Webhook channel details\",\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"required\": [\n          \"urls\",\n          \"authType\",\n          \"token\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"urls\": {\n            \"description\"\
  : \"List of Webhook URLs - do not include token in the URL\",\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"authType\": {\n            \"description\": \"Webhook Authentication Type\",\n            \"type\": \"string\",\n            \"enum\": [\n              \"NO_AUTH\",\n              \"TOKEN\"\n            ]\n          },\n          \"token\": {\n            \"description\": \"Webhook token value\",\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"template\": {\n      \"description\": \"Channel output template\",\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"description\": \"Output channel template name\",\n          \"type\": \"string\"\n        },\n        \"templateJson\": {\n          \"description\": \"JSON describing the output channel template\",\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n\
  \  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-channel-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifChannel
---
