---
description: NotifListApiReqBody schema from Multi-Tenant Notifications API
layout: schema
name: NotifListApiReqBody
properties_list:
- description: List of output channels that the notification is sent on
  name: filters
  type: array
- description: List of output channels that the notification is sent on
  name: sortByList
  type: array
- description: Page number
  name: page
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-list-api-req-body-schema.json
slug: sase-multitenant-notifications-api-notif-list-api-req-body
source_filename: sase-multitenant-notifications-api-notif-list-api-req-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifListApiReqBody\",\n  \"description\": \"NotifListApiReqBody schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-list-api-req-body-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"description\": \"List of output channels that the notification is sent on\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"field\": {\n            \"description\": \"Filter field\",\n            \"type\": \"string\"\n          },\n          \"values\": {\n            \"description\": \"Filter field values\",\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"readState\"\
  ,\n                \"notifType\",\n                \"category\",\n                \"subCategory\",\n                \"inApp\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"sortByList\": {\n      \"description\": \"List of output channels that the notification is sent on\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"field\": {\n            \"description\": \"Sort field\",\n            \"type\": \"string\",\n            \"enum\": [\n              \"createdTime\",\n              \"impactedTenantCount\"\n            ]\n          },\n          \"sortBy\": {\n            \"description\": \"Ascending or Descending\",\n            \"type\": \"string\",\n            \"enum\": [\n              \"DESC\",\n              \"ASC\"\n            ]\n          }\n        }\n      }\n    },\n    \"page\": {\n      \"type\": \"object\",\n      \"description\": \"Page number\",\n      \"properties\"\
  : {\n        \"num\": {\n          \"type\": \"integer\",\n          \"description\": \"Page number\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"description\": \"Page size\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-list-api-req-body-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifListApiReqBody
---
