---
description: Subscription list operation response.
layout: schema
name: SubscriptionListResult
properties_list:
- description: An array of subscriptions.
  name: value
  type: array
- description: The URL to get the next set of results.
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-resource-manager-subscription-list-result-schema.json
slug: azure-resource-manager-subscription-list-result
source_filename: azure-resource-manager-subscription-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionListResult\",\n  \"type\": \"object\",\n  \"description\": \"Subscription list operation response.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"An array of subscriptions.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to get the next set of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-resource-manager-subscription-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: SubscriptionListResult
---
