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
schema_file: json-schema/crm-feature-flags-api-portal-flag-state-collection-schema.json
slug: crm-feature-flags-api-portal-flag-state-collection
source_filename: crm-feature-flags-api-portal-flag-state-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-portal-flag-state-collection-schema.json\",\n  \"title\": \"PortalFlagStateCollection\",\n  \"description\": \"A paginated collection of portal flag states\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portalFlagStates\": {\n      \"type\": \"array\",\n      \"description\": \"List of portal flag states\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents the flag state override for a specific portal (account)\",\n        \"required\": [\n          \"appId\",\n          \"flagName\",\n          \"portalId\",\n          \"flagState\"\n        ],\n        \"properties\": {\n          \"appId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot application\"\
  ,\n            \"example\": 12345678\n          },\n          \"flagName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the feature flag\",\n            \"example\": \"new-dashboard-feature\"\n          },\n          \"portalId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The unique identifier for the HubSpot portal (account)\",\n            \"example\": 98765432\n          },\n          \"flagState\": {\n            \"$ref\": \"#/components/schemas/FlagState\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"appId\": 12345678,\n          \"flagName\": \"new-dashboard-feature\",\n          \"portalId\": 98765432,\n          \"flagState\": {}\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for list responses\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\"\
  ,\n          \"description\": \"Information for fetching the next page of results\",\n          \"required\": [\n            \"after\"\n          ],\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\",\n              \"example\": \"NTI1Cg%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Direct link to the next page\",\n              \"example\": \"https://api.hubapi.com/feature-flags/v3/12345678/flags/new-dashboard-feature/portals?after=NTI1Cg%3D%3D\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"portalFlagStates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-feature-flags-api-portal-flag-state-collection-schema.json
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
