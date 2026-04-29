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
schema_file: json-schema/hubspot-crm-feature-flags-feature-flag-input-schema.json
slug: hubspot-crm-feature-flags-feature-flag-input
source_filename: hubspot-crm-feature-flags-feature-flag-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input payload for creating or updating a feature flag\",\n  \"properties\": {\n    \"defaultState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of a feature flag\",\n      \"example\": \"ON\",\n      \"enum\": [\n        \"ON\",\n        \"OFF\",\n        \"ABSENT\"\n      ]\n    }\n  },\n  \"required\": [\n    \"defaultState\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FeatureFlagInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-feature-flag-input-schema.json
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
