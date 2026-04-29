---
description: A paginated collection of portal flag states
layout: schema
name: PortalFlagStateCollection
properties_list:
- description: List of portal flag states
  name: portalFlagStates
  type: array
- description: Pagination information for list responses
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-portal-flag-state-collection-schema.json
slug: hubspot-crm-feature-flags-portal-flag-state-collection
source_filename: hubspot-crm-feature-flags-portal-flag-state-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of portal flag states\",\n  \"properties\": {\n    \"portalFlagStates\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag states\",\n      \"example\": [\n        {\n          \"appId\": 12345678,\n          \"flagName\": \"new-dashboard-feature\",\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents the flag state override for a specific portal (account)\",\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier for the HubSpot application\",\n            \"format\": \"int64\",\n            \"example\": 12345678\n          },\n          \"flagName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the feature flag\",\n            \"example\"\
  : \"new-dashboard-feature\"\n          },\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"format\": \"int64\",\n            \"example\": 98765432\n          },\n          \"flagState\": {\n            \"type\": \"string\",\n            \"description\": \"The state of a feature flag\",\n            \"example\": \"ON\",\n            \"enum\": [\n              \"ON\",\n              \"OFF\",\n              \"ABSENT\"\n            ]\n          }\n        },\n        \"required\": [\n          \"appId\",\n          \"flagName\",\n          \"portalId\",\n          \"flagState\"\n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for list responses\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Information for fetching the next page of results\"\
  ,\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\",\n              \"example\": \"NTI1Cg%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Direct link to the next page\",\n              \"example\": \"https://api.hubapi.com/feature-flags/v3/12345678/flags/new-dashboard-feature/portals?after=NTI1Cg%3D%3D\"\n            }\n          },\n          \"required\": [\n            \"after\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"portalFlagStates\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PortalFlagStateCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-portal-flag-state-collection-schema.json
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
title: PortalFlagStateCollection
---
