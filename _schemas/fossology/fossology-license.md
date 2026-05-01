---
description: A license record as represented inside FOSSology.
layout: schema
name: FOSSologyLicense
properties_list:
- description: ''
  name: id
  type: integer
- description: SPDX-style short identifier (e.g., GPL-2.0-only).
  name: shortName
  type: string
- description: ''
  name: fullName
  type: string
- description: Full license text.
  name: text
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: risk
  type: integer
- description: ''
  name: isCandidate
  type: boolean
- description: References to obligation ids.
  name: obligations
  type: array
provider_name: FOSSology
provider_slug: fossology
schema_file: json-schema/fossology-license.json
slug: fossology-license
source_filename: fossology-license.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/json-schema/fossology-license.json\",\n  \"title\": \"FOSSologyLicense\",\n  \"description\": \"A license record as represented inside FOSSology.\",\n  \"type\": \"object\",\n  \"required\": [\"shortName\"],\n  \"properties\": {\n    \"id\": { \"type\": \"integer\" },\n    \"shortName\": { \"type\": \"string\", \"description\": \"SPDX-style short identifier (e.g., GPL-2.0-only).\" },\n    \"fullName\": { \"type\": \"string\" },\n    \"text\": { \"type\": \"string\", \"description\": \"Full license text.\" },\n    \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"risk\": { \"type\": \"integer\", \"minimum\": 0, \"maximum\": 5 },\n    \"isCandidate\": { \"type\": \"boolean\" },\n    \"obligations\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"integer\" },\n      \"description\": \"References\
  \ to obligation ids.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/json-schema/fossology-license.json
tags:
- Compliance
- Licensing
- Linux Foundation
- Scanning
- SPDX
- Open Source
title: FOSSologyLicense
---
