---
description: NotifStateChangeApiBody schema from Multi-Tenant Notifications API
layout: schema
name: NotifStateChangeApiBody
properties_list:
- description: List of notification IDs
  name: notifIds
  type: array
- description: Read state of the notification
  name: readState
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-state-change-api-body-schema.json
slug: sase-multitenant-notifications-api-notif-state-change-api-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifStateChangeApiBody\",\n  \"description\": \"NotifStateChangeApiBody schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-state-change-api-body-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notifIds\": {\n      \"description\": \"List of notification IDs\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"readState\": {\n      \"type\": \"string\",\n      \"description\": \"Read state of the notification\",\n      \"enum\": [\n        \"READ\",\n        \"UNREAD\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-state-change-api-body-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifStateChangeApiBody
---
