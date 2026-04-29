---
description: Input payload for creating or updating a feature flag
layout: schema
name: FeatureFlagInput
properties_list:
- description: The state of a feature flag
  name: defaultState
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-feature-flags-api-feature-flag-input-schema.json
slug: crm-feature-flags-api-feature-flag-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-feature-flag-input-schema.json\",\n  \"title\": \"FeatureFlagInput\",\n  \"description\": \"Input payload for creating or updating a feature flag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of a feature flag\",\n      \"enum\": [\n        \"ON\",\n        \"OFF\",\n        \"ABSENT\"\n      ],\n      \"example\": \"ON\"\n    }\n  },\n  \"required\": [\n    \"defaultState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-feature-flag-input-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: FeatureFlagInput
---
