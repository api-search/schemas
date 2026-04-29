---
description: SubscriptionEntitlements schema from Palo Alto Networks SASE Subscription Service API
layout: schema
name: SubscriptionEntitlements
properties_list:
- description: Unique identifier of the subscription.
  name: subscription_id
  type: string
- description: Product name.
  name: product_name
  type: string
- description: Granular entitlements included in the subscription.
  name: entitlements
  type: array
- description: Current license allocations by child TSG.
  name: allocations
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-subscription-api-subscription-entitlements-schema.json
slug: sase-subscription-api-subscription-entitlements
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionEntitlements\",\n  \"description\": \"SubscriptionEntitlements schema from Palo Alto Networks SASE Subscription Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-subscription-entitlements-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscription_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the subscription.\"\n    },\n    \"product_name\": {\n      \"type\": \"string\",\n      \"description\": \"Product name.\"\n    },\n    \"entitlements\": {\n      \"type\": \"array\",\n      \"description\": \"Granular entitlements included in the subscription.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"feature\": {\n            \"type\": \"string\",\n            \"description\": \"Feature\
  \ or capability name.\"\n          },\n          \"licensed_quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Licensed quantity for this entitlement.\"\n          },\n          \"allocated_quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Quantity already allocated to child TSGs.\"\n          },\n          \"available_quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Remaining quantity available for allocation.\"\n          },\n          \"unit\": {\n            \"type\": \"string\",\n            \"description\": \"Unit of measure.\"\n          }\n        }\n      }\n    },\n    \"allocations\": {\n      \"type\": \"array\",\n      \"description\": \"Current license allocations by child TSG.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tsg_id\": {\n            \"type\": \"string\",\n            \"description\": \"Child TSG ID receiving this allocation.\"\
  \n          },\n          \"tsg_name\": {\n            \"type\": \"string\",\n            \"description\": \"Display name of the child TSG.\"\n          },\n          \"allocated_quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Quantity allocated to this TSG.\"\n          },\n          \"utilized_quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Quantity currently utilized by this TSG.\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-subscription-entitlements-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SubscriptionEntitlements
---
