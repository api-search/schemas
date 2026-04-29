---
description: NotifCategoryDetail schema from Multi-Tenant Notifications API
layout: schema
name: NotifCategoryDetail
properties_list:
- description: Notification type category name
  name: name
  type: string
- description: Best practice flag for category
  name: bestPractice
  type: boolean
- description: List of notification type sub-categories
  name: subCategoryList
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-category-detail-schema.json
slug: sase-multitenant-notifications-api-notif-category-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifCategoryDetail\",\n  \"description\": \"NotifCategoryDetail schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-category-detail-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Notification type category name\",\n      \"type\": \"string\"\n    },\n    \"bestPractice\": {\n      \"description\": \"Best practice flag for category\",\n      \"type\": \"boolean\"\n    },\n    \"subCategoryList\": {\n      \"description\": \"List of notification type sub-categories\",\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"name\",\n          \"bestPractice\",\n          \"needLicense\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n        \
  \  \"name\": {\n            \"description\": \"Notification type sub-category name\",\n            \"type\": \"string\"\n          },\n          \"bestPractice\": {\n            \"description\": \"Best practice flag for sub-category\",\n            \"type\": \"boolean\"\n          },\n          \"needLicense\": {\n            \"description\": \"Need license flag for sub-category\",\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"bestPractice\",\n    \"subCategoryList\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-category-detail-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifCategoryDetail
---
