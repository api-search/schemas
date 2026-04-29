---
description: NotifSubCategoryDetail schema from Multi-Tenant Notifications API
layout: schema
name: NotifSubCategoryDetail
properties_list:
- description: Notification type sub-category name
  name: name
  type: string
- description: Best practice flag for sub-category
  name: bestPractice
  type: boolean
- description: Need license flag for sub-category
  name: needLicense
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-sub-category-detail-schema.json
slug: sase-multitenant-notifications-api-notif-sub-category-detail
source_filename: sase-multitenant-notifications-api-notif-sub-category-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifSubCategoryDetail\",\n  \"description\": \"NotifSubCategoryDetail schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-sub-category-detail-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Notification type sub-category name\",\n      \"type\": \"string\"\n    },\n    \"bestPractice\": {\n      \"description\": \"Best practice flag for sub-category\",\n      \"type\": \"boolean\"\n    },\n    \"needLicense\": {\n      \"description\": \"Need license flag for sub-category\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"bestPractice\",\n    \"needLicense\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-sub-category-detail-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifSubCategoryDetail
---
