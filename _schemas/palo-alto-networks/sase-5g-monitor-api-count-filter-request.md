---
description: CountFilterRequest schema from SASE 5G Monitor Service API
layout: schema
name: CountFilterRequest
properties_list:
- description: ''
  name: filter
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-monitor-api-count-filter-request-schema.json
slug: sase-5g-monitor-api-count-filter-request
source_filename: sase-5g-monitor-api-count-filter-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CountFilterRequest\",\n  \"description\": \"CountFilterRequest schema from SASE 5G Monitor Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-monitor-api-count-filter-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"operator\": {\n          \"type\": \"string\"\n        },\n        \"rules\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"property\": {\n                \"type\": \"string\"\n              },\n              \"operator\": {\n                \"type\": \"string\"\n              },\n              \"values\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\":\
  \ \"object\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-monitor-api-count-filter-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CountFilterRequest
---
