---
description: A billing policy that defines the association between an Azure subscription and Power Platform environments for pay-as-you-go billing.
layout: schema
name: BillingPolicy
properties_list:
- description: The unique identifier of the billing policy.
  name: id
  type: string
- description: The display name of the billing policy.
  name: name
  type: string
- description: The geographic location of the billing policy.
  name: location
  type: string
- description: The status of the billing policy.
  name: status
  type: string
- description: The timestamp when the billing policy was created.
  name: createdOn
  type: string
- description: The timestamp of the last modification.
  name: lastModifiedOn
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-billing-policy-schema.json
slug: power-platform-billing-policy
source_filename: power-platform-billing-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillingPolicy\",\n  \"type\": \"object\",\n  \"description\": \"A billing policy that defines the association between an Azure subscription and Power Platform environments for pay-as-you-go billing.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the billing policy.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the billing policy.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic location of the billing policy.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the billing policy.\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the billing policy was created.\"\n    },\n    \"lastModifiedOn\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The timestamp of the last modification.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-billing-policy-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: BillingPolicy
---
