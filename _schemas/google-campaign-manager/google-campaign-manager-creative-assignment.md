---
description: Creative assignment within a creative rotation.
layout: schema
name: CreativeAssignment
properties_list:
- description: ID of the creative to be assigned.
  name: creativeId
  type: string
- description: Whether this creative assignment is active.
  name: active
  type: boolean
- description: Weight of the creative assignment.
  name: weight
  type: integer
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: Sequence number of the creative assignment.
  name: sequence
  type: integer
- description: ''
  name: richMediaExitOverrides
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-creative-assignment-schema.json
slug: google-campaign-manager-creative-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreativeAssignment\",\n  \"type\": \"object\",\n  \"description\": \"Creative assignment within a creative rotation.\",\n  \"properties\": {\n    \"creativeId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the creative to be assigned.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this creative assignment is active.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight of the creative assignment.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"sequence\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequence number of the creative assignment.\"\n    },\n    \"richMediaExitOverrides\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-creative-assignment-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: CreativeAssignment
---
