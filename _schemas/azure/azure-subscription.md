---
description: Subscription information.
layout: schema
name: Subscription
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: subscriptionId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: subscriptionPolicies
  type: object
- description: ''
  name: authorizationSource
  type: string
- description: ''
  name: managedByTenants
  type: array
provider_name: Microsoft Azure
provider_slug: azure
schema_file: json-schema/azure-subscription-schema.json
slug: azure-subscription
source_filename: azure-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/json-schema/azure-subscription-schema.json\",\n  \"title\": \"Subscription\",\n  \"description\": \"Subscription information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Enabled\",\n        \"Disabled\",\n        \"Deleted\",\n        \"PastDue\",\n        \"Warned\"\n      ]\n    },\n    \"subscriptionPolicies\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"locationPlacementId\": {\n          \"type\": \"string\"\n        },\n        \"quotaId\": {\n          \"type\": \"string\"\n        },\n   \
  \     \"spendingLimit\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"On\",\n            \"Off\",\n            \"CurrentPeriodOff\"\n          ]\n        }\n      }\n    },\n    \"authorizationSource\": {\n      \"type\": \"string\"\n    },\n    \"managedByTenants\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tenantId\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure/refs/heads/main/json-schema/azure-subscription-schema.json
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Platform as a Service
- Storage
title: Subscription
---
