---
description: A service object defining a TCP or UDP protocol with destination port or port range.
layout: schema
name: Service
properties_list:
- description: Unique name of the service object.
  name: '@name'
  type: string
- description: ''
  name: protocol
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: tag
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/pan-os-rest-api-service-schema.json
slug: pan-os-rest-api-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"description\": \"A service object defining a TCP or UDP protocol with destination port or port range.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-service-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the service object.\"\n    },\n    \"protocol\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tcp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\",\n              \"description\": \"TCP destination port or range (e.g., 80, 8080-8090).\"\n            },\n            \"source-port\": {\n              \"type\": \"string\",\n              \"description\": \"TCP source port or range.\"\n            }\n\
  \          }\n        },\n        \"udp\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\",\n              \"description\": \"UDP destination port or range (e.g., 53, 500-502).\"\n            },\n            \"source-port\": {\n              \"type\": \"string\",\n              \"description\": \"UDP source port or range.\"\n            }\n          }\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"member\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/pan-os-rest-api-service-schema.json
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
