---
description: ServiceList schema from Palo Alto Networks Strata Cloud Manager API
layout: schema
name: ServiceList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: offset
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-service-list-schema.json
slug: strata-cloud-manager-api-service-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceList\",\n  \"description\": \"ServiceList schema from Palo Alto Networks Strata Cloud Manager API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-service-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A service object defining a protocol and port combination for use in security policy rules.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\",\n            \"readOnly\": true\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"folder\": {\n            \"type\": \"string\",\n            \"readOnly\": true\n          },\n          \"protocol\": {\n\
  \            \"type\": \"object\",\n            \"properties\": {\n              \"tcp\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"port\": {\n                    \"type\": \"string\",\n                    \"description\": \"TCP destination port or range (e.g., 80, 8080-8090).\"\n                  },\n                  \"source_port\": {\n                    \"type\": \"string\"\n                  }\n                }\n              },\n              \"udp\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"port\": {\n                    \"type\": \"string\",\n                    \"description\": \"UDP destination port or range (e.g., 53).\"\n                  },\n                  \"source_port\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"description\": {\n            \"type\": \"string\"\
  \n          },\n          \"tag\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-service-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceList
---
