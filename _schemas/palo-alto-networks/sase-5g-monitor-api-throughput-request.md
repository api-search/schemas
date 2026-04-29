---
description: ThroughputRequest schema from SASE 5G Monitor Service API
layout: schema
name: ThroughputRequest
properties_list:
- description: ''
  name: properties
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: histogram
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-monitor-api-throughput-request-schema.json
slug: sase-5g-monitor-api-throughput-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThroughputRequest\",\n  \"description\": \"ThroughputRequest schema from SASE 5G Monitor Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-monitor-api-throughput-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"property\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"operator\": {\n          \"type\": \"string\"\n        },\n        \"rules\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"property\": {\n                \"type\": \"string\"\n  \
  \            },\n              \"operator\": {\n                \"type\": \"string\"\n              },\n              \"values\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"histogram\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"property\": {\n          \"type\": \"string\"\n        },\n        \"range\": {\n          \"type\": \"string\"\n        },\n        \"enableEmptyInterval\": {\n          \"type\": \"boolean\"\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-monitor-api-throughput-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ThroughputRequest
---
