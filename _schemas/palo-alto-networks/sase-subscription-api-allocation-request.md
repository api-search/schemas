---
description: AllocationRequest schema from Palo Alto Networks SASE Subscription Service API
layout: schema
name: AllocationRequest
properties_list:
- description: Array of TSG allocations to set. Each entry specifies a child TSG and the quantity to allocate to it. Existing allocations for TSGs not included in the array are unchanged.
  name: allocations
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-subscription-api-allocation-request-schema.json
slug: sase-subscription-api-allocation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AllocationRequest\",\n  \"description\": \"AllocationRequest schema from Palo Alto Networks SASE Subscription Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-allocation-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allocations\": {\n      \"type\": \"array\",\n      \"description\": \"Array of TSG allocations to set. Each entry specifies a child TSG and the quantity to allocate to it. Existing allocations for TSGs not included in the array are unchanged.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"tsg_id\",\n          \"quantity\"\n        ],\n        \"properties\": {\n          \"tsg_id\": {\n            \"type\": \"string\",\n            \"description\": \"Child TSG ID to allocate licenses to.\"\n          },\n   \
  \       \"quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of licenses to allocate to this TSG.\",\n            \"minimum\": 0\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"allocations\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-subscription-api-allocation-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AllocationRequest
---
