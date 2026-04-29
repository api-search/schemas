---
description: MtNotifAggKey schema from Multi-Tenant Notifications API
layout: schema
name: MtNotifAggKey
properties_list:
- description: TSG Id
  name: tsgId
  type: string
- description: Notification Type
  name: notifType
  type: string
- description: Notification category - is associated with notification type
  name: category
  type: string
- description: Notification sub-category - is associated with notification type and notification category
  name: subCategory
  type: string
- description: InApp Notification Flag
  name: inAppFlag
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-mt-notif-agg-key-schema.json
slug: sase-multitenant-notifications-api-mt-notif-agg-key
source_filename: sase-multitenant-notifications-api-mt-notif-agg-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MtNotifAggKey\",\n  \"description\": \"MtNotifAggKey schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-mt-notif-agg-key-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsgId\": {\n      \"description\": \"TSG Id\",\n      \"type\": \"string\"\n    },\n    \"notifType\": {\n      \"description\": \"Notification Type\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"INCIDENTS\",\n        \"UPGRADES\",\n        \"ANNOUNCEMENTS\"\n      ]\n    },\n    \"category\": {\n      \"description\": \"Notification category - is associated with notification type\",\n      \"type\": \"string\"\n    },\n    \"subCategory\": {\n      \"description\": \"Notification sub-category - is associated with notification type and notification category\"\
  ,\n      \"type\": \"string\"\n    },\n    \"inAppFlag\": {\n      \"description\": \"InApp Notification Flag\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"tsgId\",\n    \"notifType\",\n    \"category\",\n    \"subCategory\",\n    \"inAppFlag\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-mt-notif-agg-key-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MtNotifAggKey
---
