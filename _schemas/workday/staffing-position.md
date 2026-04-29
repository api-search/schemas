---
description: ''
layout: schema
name: Position
properties_list:
- description: The Workday ID of the position.
  name: id
  type: string
- description: A display descriptor for the position.
  name: descriptor
  type: string
- description: The position reference ID.
  name: positionID
  type: string
- description: Whether the position is currently filled.
  name: isFilled
  type: boolean
- description: Whether the position is available for recruiting.
  name: isAvailableForRecruit
  type: boolean
- description: Whether the position has been closed.
  name: isClosed
  type: boolean
provider_name: Workday
provider_slug: workday
schema_file: json-schema/staffing-position-schema.json
slug: staffing-position
source_filename: staffing-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Position\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the position.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the position.\"\n    },\n    \"positionID\": {\n      \"type\": \"string\",\n      \"description\": \"The position reference ID.\"\n    },\n    \"isFilled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is currently filled.\"\n    },\n    \"isAvailableForRecruit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position is available for recruiting.\"\n    },\n    \"isClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the position has been closed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/staffing-position-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Position
---
