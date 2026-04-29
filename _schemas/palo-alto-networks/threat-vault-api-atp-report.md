---
description: Advanced Threat Prevention inline analysis report.
layout: schema
name: AtpReport
properties_list:
- description: Unique report identifier.
  name: id
  type: string
- description: SHA-256 hash of the analyzed sample.
  name: sha256
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: verdict
  type: string
- description: ''
  name: create_time
  type: string
- description: Detailed behavioral analysis data.
  name: report
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/threat-vault-api-atp-report-schema.json
slug: threat-vault-api-atp-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AtpReport\",\n  \"description\": \"Advanced Threat Prevention inline analysis report.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-atp-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique report identifier.\"\n    },\n    \"sha256\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 hash of the analyzed sample.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"complete\",\n        \"error\"\n      ]\n    },\n    \"verdict\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"benign\",\n        \"malware\",\n        \"grayware\",\n        \"phishing\",\n        \"unknown\"\n      ]\n    },\n    \"create_time\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\"\n    },\n    \"report\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed behavioral analysis data.\",\n      \"properties\": {\n        \"file_type\": {\n          \"type\": \"string\"\n        },\n        \"size\": {\n          \"type\": \"integer\"\n        },\n        \"behaviors\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"description\": {\n                \"type\": \"string\"\n              },\n              \"severity\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"network\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"dns_queries\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n\
  \            },\n            \"http_requests\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"connections\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"dst_ip\": {\n                    \"type\": \"string\"\n                  },\n                  \"dst_port\": {\n                    \"type\": \"integer\"\n                  },\n                  \"protocol\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-atp-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AtpReport
---
