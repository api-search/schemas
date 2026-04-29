---
description: Subscription policies.
layout: schema
name: SubscriptionPolicies
properties_list:
- description: The subscription location placement ID.
  name: locationPlacementId
  type: string
- description: The subscription quota ID.
  name: quotaId
  type: string
- description: The subscription spending limit.
  name: spendingLimit
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-subscription-policies-schema.json
slug: azure-resource-manager-subscription-policies
source_filename: azure-resource-manager-subscription-policies-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionPolicies\",\n  \"type\": \"object\",\n  \"description\": \"Subscription policies.\",\n  \"properties\": {\n    \"locationPlacementId\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription location placement ID.\"\n    },\n    \"quotaId\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription quota ID.\"\n    },\n    \"spendingLimit\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription spending limit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-subscription-policies-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: SubscriptionPolicies
---
