---
description: A Red Hat subscription providing product entitlements for an organization.
layout: schema
name: Subscription
properties_list:
- description: Unique identifier for the subscription.
  name: id
  type: integer
- description: Candlepin subscription identifier.
  name: cp_id
  type: string
- description: Subscription pool identifier.
  name: subscription_id
  type: integer
- description: Subscription name (product name).
  name: name
  type: string
- description: Subscription description.
  name: description
  type: '[''string'', ''null'']'
- description: Red Hat product identifier.
  name: product_id
  type: string
- description: Red Hat product name.
  name: product_name
  type: string
- description: Contract number associated with the subscription.
  name: contract_number
  type: '[''string'', ''null'']'
- description: Customer account number.
  name: account_number
  type: '[''string'', ''null'']'
- description: Total quantity of entitlements in the subscription.
  name: quantity
  type: integer
- description: Number of entitlements currently consumed.
  name: consumed
  type: integer
- description: Number of entitlements available for attachment.
  name: available
  type: integer
- description: Subscription start date.
  name: start_date
  type: string
- description: Subscription end date.
  name: end_date
  type: string
- description: Support level (e.g., Premium, Standard, Self-Support).
  name: support_level
  type: '[''string'', ''null'']'
- description: Subscription type.
  name: type
  type: string
- description: Whether this subscription is for virtual systems only.
  name: virt_only
  type: boolean
- description: Whether this subscription requires virt-who reporting.
  name: virt_who
  type: boolean
- description: Whether multiple entitlements can be attached to a single host.
  name: multi_entitlement
  type: boolean
- description: Stacking identifier for stackable subscriptions.
  name: stacking_id
  type: '[''string'', ''null'']'
- description: Pool identifier from the upstream subscription source.
  name: upstream_pool_id
  type: '[''string'', ''null'']'
- description: Organization this subscription belongs to.
  name: organization_id
  type: integer
- description: Products provided by this subscription.
  name: provided_products
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-subscription-schema.json
slug: red-hat-satellite-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"description\": \"A Red Hat subscription providing product entitlements for an organization.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the subscription.\"\n    },\n    \"cp_id\": {\n      \"type\": \"string\",\n      \"description\": \"Candlepin subscription identifier.\"\n    },\n    \"subscription_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Subscription pool identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription name (product name).\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Subscription description.\"\n    },\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"Red Hat product identifier.\"\n    },\n    \"product_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Red Hat product name.\"\n    },\n    \"contract_number\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Contract number associated with the subscription.\"\n    },\n    \"account_number\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Customer account number.\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total quantity of entitlements in the subscription.\"\n    },\n    \"consumed\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of entitlements currently consumed.\"\n    },\n    \"available\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of entitlements available for attachment.\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription start date.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription end date.\"\n   \
  \ },\n    \"support_level\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Support level (e.g., Premium, Standard, Self-Support).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription type.\"\n    },\n    \"virt_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this subscription is for virtual systems only.\"\n    },\n    \"virt_who\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this subscription requires virt-who reporting.\"\n    },\n    \"multi_entitlement\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether multiple entitlements can be attached to a single host.\"\n    },\n    \"stacking_id\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Stacking identifier for stackable subscriptions.\"\n    },\n    \"upstream_pool_id\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Pool identifier from the upstream subscription\
  \ source.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization this subscription belongs to.\"\n    },\n    \"provided_products\": {\n      \"type\": \"array\",\n      \"description\": \"Products provided by this subscription.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-subscription-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: Subscription
---
