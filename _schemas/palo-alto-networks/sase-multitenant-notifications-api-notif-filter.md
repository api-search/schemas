---
description: NotifFilter schema from Multi-Tenant Notifications API
layout: schema
name: NotifFilter
properties_list:
- description: Filter field
  name: field
  type: string
- description: Filter field values
  name: values
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-filter-schema.json
slug: sase-multitenant-notifications-api-notif-filter
source_filename: sase-multitenant-notifications-api-notif-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifFilter\",\n  \"description\": \"NotifFilter schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-filter-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"description\": \"Filter field\",\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"description\": \"Filter field values\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"readState\",\n          \"notifType\",\n          \"category\",\n          \"subCategory\",\n          \"inApp\"\n        ]\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-filter-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifFilter
---
