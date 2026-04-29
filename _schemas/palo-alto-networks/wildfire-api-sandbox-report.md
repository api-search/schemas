---
description: Analysis results from a single sandbox execution environment.
layout: schema
name: SandboxReport
properties_list:
- description: Platform identifier (e.g., 100 for Windows XP SP3).
  name: platform
  type: string
- description: Sandbox software environment.
  name: software
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: summary
  type: object
- description: ''
  name: network
  type: object
- description: ''
  name: process_list
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/wildfire-api-sandbox-report-schema.json
slug: wildfire-api-sandbox-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SandboxReport\",\n  \"description\": \"Analysis results from a single sandbox execution environment.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-sandbox-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Platform identifier (e.g., 100 for Windows XP SP3).\"\n    },\n    \"software\": {\n      \"type\": \"string\",\n      \"description\": \"Sandbox software environment.\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"@verdict\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"benign\",\n            \"malware\",\n            \"grayware\",\n            \"phishing\"\n          ]\n        }\n      }\n\
  \    },\n    \"network\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dns\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"@query\": {\n                \"type\": \"string\"\n              },\n              \"@response\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"tcp\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"@ip\": {\n                \"type\": \"string\"\n              },\n              \"@port\": {\n                \"type\": \"integer\"\n              },\n              \"@country\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"http\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"@request\": {\n                \"type\": \"string\"\n              },\n              \"@response\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"process_list\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"process\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"@name\": {\n                \"type\": \"string\"\n              },\n              \"@pid\": {\n                \"type\": \"string\"\n              },\n              \"@text\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/wildfire-api-sandbox-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SandboxReport
---
