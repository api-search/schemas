---
description: A key-value pair for a baseline parameter.
layout: schema
name: EnabledBaselineParameter
properties_list:
- description: The parameter key.
  name: key
  type: string
- description: The parameter value.
  name: value
  type: object
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enabled-baseline-parameter-schema.json
slug: enabled-baseline-parameter
source_filename: enabled-baseline-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-baseline-parameter-schema.json\",\n  \"title\": \"EnabledBaselineParameter\",\n  \"description\": \"A key-value pair for a baseline parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter key.\",\n      \"example\": \"IdentityCenterEnabled\"\n    },\n    \"value\": {\n      \"description\": \"The parameter value.\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-baseline-parameter-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnabledBaselineParameter
---
