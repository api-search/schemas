---
description: Subscription information.
layout: schema
name: Subscription
properties_list:
- description: The fully qualified ID for the subscription.
  name: id
  type: string
- description: The subscription ID.
  name: subscriptionId
  type: string
- description: The subscription display name.
  name: displayName
  type: string
- description: The subscription tenant ID.
  name: tenantId
  type: string
- description: The subscription state.
  name: state
  type: string
- description: The authorization source of the request. Valid values are one or more combinations of Legacy, RoleBased, Bypassed, Direct, Management.
  name: authorizationSource
  type: string
- description: The tags attached to the subscription.
  name: tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-subscription-schema.json
slug: azure-resource-manager-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"description\": \"Subscription information.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified ID for the subscription.\"\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription ID.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription display name.\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription tenant ID.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The subscription state.\"\n    },\n    \"authorizationSource\": {\n      \"type\": \"string\",\n      \"description\": \"The authorization source of the request. Valid values are one or more combinations of Legacy, RoleBased, Bypassed, Direct, Management.\"\
  \n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags attached to the subscription.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-subscription-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Subscription
---
