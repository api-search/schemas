---
description: Subscription schema from Palo Alto Networks SASE Subscription Service API
layout: schema
name: Subscription
properties_list:
- description: Unique identifier of the subscription.
  name: subscription_id
  type: string
- description: Tenant Service Group ID this subscription is associated with.
  name: tsg_id
  type: string
- description: Product name (e.g., Prisma Access, Prisma SD-WAN).
  name: product_name
  type: string
- description: Product SKU identifier.
  name: sku
  type: string
- description: Current subscription status.
  name: status
  type: string
- description: Total licensed quantity (e.g., number of users or devices).
  name: licensed_quantity
  type: integer
- description: Unit of measure for the licensed quantity (e.g., users, devices, Mbps).
  name: licensed_unit
  type: string
- description: Currently utilized quantity.
  name: utilized_quantity
  type: integer
- description: Subscription start date.
  name: start_date
  type: string
- description: Subscription end date.
  name: end_date
  type: string
- description: Support tier included with the subscription.
  name: support_level
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-subscription-api-subscription-schema.json
slug: sase-subscription-api-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"description\": \"Subscription schema from Palo Alto Networks SASE Subscription Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-subscription-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscription_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the subscription.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group ID this subscription is associated with.\"\n    },\n    \"product_name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name (e.g., Prisma Access, Prisma SD-WAN).\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"Product SKU identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"active\",\n        \"expired\",\n        \"pending\"\n      ],\n      \"description\": \"Current subscription status.\"\n    },\n    \"licensed_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total licensed quantity (e.g., number of users or devices).\"\n    },\n    \"licensed_unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure for the licensed quantity (e.g., users, devices, Mbps).\"\n    },\n    \"utilized_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Currently utilized quantity.\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Subscription start date.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Subscription end date.\"\n    },\n    \"support_level\": {\n      \"type\": \"string\",\n      \"description\": \"Support tier included with the subscription.\"\n   \
  \ }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-subscription-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Subscription
---
