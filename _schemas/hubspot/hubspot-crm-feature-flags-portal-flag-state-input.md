---
description: Input payload for setting a portal flag state
layout: schema
name: PortalFlagStateInput
properties_list:
- description: The state of a feature flag
  name: flagState
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-portal-flag-state-input-schema.json
slug: hubspot-crm-feature-flags-portal-flag-state-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input payload for setting a portal flag state\",\n  \"properties\": {\n    \"flagState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of a feature flag\",\n      \"example\": \"ON\",\n      \"enum\": [\n        \"ON\",\n        \"OFF\",\n        \"ABSENT\"\n      ]\n    }\n  },\n  \"required\": [\n    \"flagState\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PortalFlagStateInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-portal-flag-state-input-schema.json
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
title: PortalFlagStateInput
---
