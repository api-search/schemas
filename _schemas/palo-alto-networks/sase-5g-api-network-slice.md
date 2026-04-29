---
description: NetworkSlice schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: NetworkSlice
properties_list:
- description: Unique identifier of the network slice.
  name: slice_id
  type: string
- description: Display name of the network slice.
  name: name
  type: string
- description: Description of the slice's purpose or use case.
  name: description
  type: string
- description: 5G slice type based on 3GPP SST values. eMBB for enhanced mobile broadband, URLLC for ultra-reliable low-latency, mMTC for massive machine-type communications.
  name: slice_type
  type: string
- description: Slice/Service Type numeric value (1=eMBB, 2=URLLC, 3=mMTC).
  name: sst
  type: integer
- description: Slice Differentiator hex string for distinguishing slices of the same type.
  name: sd
  type: string
- description: Current slice status.
  name: status
  type: string
- description: ID of the security policy applied to this slice.
  name: security_policy_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-network-slice-schema.json
slug: sase-5g-api-network-slice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkSlice\",\n  \"description\": \"NetworkSlice schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-network-slice-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"slice_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the network slice.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the network slice.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the slice's purpose or use case.\"\n    },\n    \"slice_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"eMBB\",\n        \"URLLC\",\n        \"mMTC\"\n      ],\n      \"description\": \"5G slice type based on 3GPP SST values. eMBB for\
  \ enhanced mobile broadband, URLLC for ultra-reliable low-latency, mMTC for massive machine-type communications.\"\n    },\n    \"sst\": {\n      \"type\": \"integer\",\n      \"description\": \"Slice/Service Type numeric value (1=eMBB, 2=URLLC, 3=mMTC).\"\n    },\n    \"sd\": {\n      \"type\": \"string\",\n      \"description\": \"Slice Differentiator hex string for distinguishing slices of the same type.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"provisioning\",\n        \"error\"\n      ],\n      \"description\": \"Current slice status.\"\n    },\n    \"security_policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the security policy applied to this slice.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-network-slice-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NetworkSlice
---
