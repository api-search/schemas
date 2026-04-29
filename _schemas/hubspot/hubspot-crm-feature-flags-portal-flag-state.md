---
description: Represents the flag state override for a specific portal (account)
layout: schema
name: PortalFlagState
properties_list:
- description: The unique identifier for the HubSpot application
  name: appId
  type: integer
- description: The name of the feature flag
  name: flagName
  type: string
- description: The unique identifier for the HubSpot portal (account)
  name: portalId
  type: integer
- description: The state of a feature flag
  name: flagState
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-portal-flag-state-schema.json
slug: hubspot-crm-feature-flags-portal-flag-state
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents the flag state override for a specific portal (account)\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for the HubSpot application\",\n      \"format\": \"int64\",\n      \"example\": 12345678\n    },\n    \"flagName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the feature flag\",\n      \"example\": \"new-dashboard-feature\"\n    },\n    \"portalId\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for the HubSpot portal (account)\",\n      \"format\": \"int64\",\n      \"example\": 98765432\n    },\n    \"flagState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of a feature flag\",\n      \"example\": \"ON\",\n      \"enum\": [\n        \"ON\",\n        \"OFF\",\n        \"ABSENT\"\n      ]\n    }\n  },\n  \"required\": [\n    \"appId\",\n    \"flagName\",\n  \
  \  \"portalId\",\n    \"flagState\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PortalFlagState\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-portal-flag-state-schema.json
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
title: PortalFlagState
---
