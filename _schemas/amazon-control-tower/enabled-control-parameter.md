---
description: A key-value pair for a control parameter.
layout: schema
name: EnabledControlParameter
properties_list:
- description: The parameter key.
  name: key
  type: string
- description: The parameter value.
  name: value
  type: object
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/enabled-control-parameter-schema.json
slug: enabled-control-parameter
source_filename: enabled-control-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-control-parameter-schema.json\",\n  \"title\": \"EnabledControlParameter\",\n  \"description\": \"A key-value pair for a control parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter key.\",\n      \"example\": \"AllowedRegions\"\n    },\n    \"value\": {\n      \"description\": \"The parameter value.\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/enabled-control-parameter-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: EnabledControlParameter
---
