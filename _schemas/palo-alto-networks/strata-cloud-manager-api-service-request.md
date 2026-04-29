---
description: ServiceRequest schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: ServiceRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: protocol
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-service-request-schema.json
slug: strata-cloud-manager-api-service-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceRequest\",\n  \"description\": \"ServiceRequest schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-service-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"protocol\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tcp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\"\n            },\n            \"source_port\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"udp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\"\n            },\n            \"source_port\"\
  : {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"protocol\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-service-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceRequest
---
