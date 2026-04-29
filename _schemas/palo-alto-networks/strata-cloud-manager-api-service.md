---
description: A service object defining a protocol and port combination for use in security policy rules.
layout: schema
name: Service
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: folder
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
schema_file: json-schema/strata-cloud-manager-api-service-schema.json
slug: strata-cloud-manager-api-service
source_filename: strata-cloud-manager-api-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"description\": \"A service object defining a protocol and port combination for use in security policy rules.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-service-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"protocol\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tcp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\",\n              \"description\": \"TCP destination port or range (e.g., 80, 8080-8090).\"\n            },\n    \
  \        \"source_port\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"udp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\",\n              \"description\": \"UDP destination port or range (e.g., 53).\"\n            },\n            \"source_port\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-service-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Service
---
