---
description: BPARequest schema from Palo Alto Networks AIOps for NGFW BPA API
layout: schema
name: BPARequest
properties_list:
- description: Device serial number of the NGFW to assess.
  name: serial_number
  type: string
- description: PAN-OS software version running on the device (e.g., 11.1.2).
  name: version
  type: string
- description: Optional supplementary device information.
  name: device_info
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/aiops-ngfw-bpa-api-bpa-request-schema.json
slug: aiops-ngfw-bpa-api-bpa-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BPARequest\",\n  \"description\": \"BPARequest schema from Palo Alto Networks AIOps for NGFW BPA API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"Device serial number of the NGFW to assess.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"PAN-OS software version running on the device (e.g., 11.1.2).\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+(\\\\.\\\\d+)?(-h\\\\d+)?$\"\n    },\n    \"device_info\": {\n      \"type\": \"object\",\n      \"description\": \"Optional supplementary device information.\",\n      \"properties\": {\n        \"hostname\": {\n          \"type\": \"string\",\n          \"description\": \"Device hostname.\"\
  \n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"Device model (e.g., PA-5450, PA-440).\"\n        },\n        \"deployment_type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"physical\",\n            \"vm\",\n            \"container\"\n          ],\n          \"description\": \"Device deployment type.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"serial_number\",\n    \"version\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/aiops-ngfw-bpa-api-bpa-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: BPARequest
---
