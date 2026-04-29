---
description: Placement assignment for an ad.
layout: schema
name: PlacementAssignment
properties_list:
- description: ID of the placement to be assigned.
  name: placementId
  type: string
- description: Whether this placement assignment is active.
  name: active
  type: boolean
- description: Whether the placement requires SSL.
  name: sslRequired
  type: boolean
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-placement-assignment-schema.json
slug: google-campaign-manager-placement-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlacementAssignment\",\n  \"type\": \"object\",\n  \"description\": \"Placement assignment for an ad.\",\n  \"properties\": {\n    \"placementId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the placement to be assigned.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this placement assignment is active.\"\n    },\n    \"sslRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the placement requires SSL.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-placement-assignment-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: PlacementAssignment
---
