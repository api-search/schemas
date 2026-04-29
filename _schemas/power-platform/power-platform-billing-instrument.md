---
description: The billing instrument information linking to an Azure subscription.
layout: schema
name: BillingInstrument
properties_list:
- description: The identifier of the billing instrument.
  name: id
  type: string
- description: The resource group within the Azure subscription.
  name: resourceGroup
  type: string
- description: The Azure subscription ID.
  name: subscriptionId
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-billing-instrument-schema.json
slug: power-platform-billing-instrument
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillingInstrument\",\n  \"type\": \"object\",\n  \"description\": \"The billing instrument information linking to an Azure subscription.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the billing instrument.\"\n    },\n    \"resourceGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The resource group within the Azure subscription.\"\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"description\": \"The Azure subscription ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-billing-instrument-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: BillingInstrument
---
