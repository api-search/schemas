---
description: Represents a feature flag configuration for an application
layout: schema
name: FeatureFlag
properties_list:
- description: The unique identifier for the HubSpot application
  name: appId
  type: integer
- description: The name of the feature flag
  name: flagName
  type: string
- description: The state of a feature flag
  name: defaultState
  type: string
- description: The state of a feature flag
  name: overrideState
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-feature-flag-schema.json
slug: hubspot-crm-feature-flags-feature-flag
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a feature flag configuration for an application\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for the HubSpot application\",\n      \"format\": \"int64\",\n      \"example\": 12345678\n    },\n    \"flagName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the feature flag\",\n      \"example\": \"new-dashboard-feature\"\n    },\n    \"defaultState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of a feature flag\",\n      \"example\": \"ON\",\n      \"enum\": [\n        \"ON\",\n        \"OFF\",\n        \"ABSENT\"\n      ]\n    },\n    \"overrideState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of a feature flag\",\n      \"example\": \"ON\",\n      \"enum\": [\n        \"ON\",\n        \"OFF\",\n        \"ABSENT\"\n      ]\n    }\n  },\n  \"required\": [\n    \"appId\"\
  ,\n    \"flagName\",\n    \"defaultState\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FeatureFlag\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-feature-flag-schema.json
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
title: FeatureFlag
---
