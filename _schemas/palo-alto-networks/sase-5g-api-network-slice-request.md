---
description: NetworkSliceRequest schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: NetworkSliceRequest
properties_list:
- description: Display name for the network slice.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: 5G slice type.
  name: slice_type
  type: string
- description: Slice Differentiator hex string.
  name: sd
  type: string
- description: Security policy ID to apply to this slice.
  name: security_policy_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-network-slice-request-schema.json
slug: sase-5g-api-network-slice-request
source_filename: sase-5g-api-network-slice-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkSliceRequest\",\n  \"description\": \"NetworkSliceRequest schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-network-slice-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the network slice.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"slice_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"eMBB\",\n        \"URLLC\",\n        \"mMTC\"\n      ],\n      \"description\": \"5G slice type.\"\n    },\n    \"sd\": {\n      \"type\": \"string\",\n      \"description\": \"Slice Differentiator hex string.\"\n    },\n    \"security_policy_id\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Security policy ID to apply to this slice.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"slice_type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-network-slice-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NetworkSliceRequest
---
