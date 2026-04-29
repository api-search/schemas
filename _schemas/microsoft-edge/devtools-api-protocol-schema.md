---
description: DevTools Protocol schema definition from the Microsoft Edge DevTools Protocol HTTP API
layout: schema
name: ProtocolSchema
properties_list:
- description: Protocol version
  name: version
  type: object
- description: Protocol domains
  name: domains
  type: array
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/devtools-api-protocol-schema-schema.json
slug: devtools-api-protocol-schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/devtools-api-protocol-schema-schema.json\",\n  \"title\": \"ProtocolSchema\",\n  \"description\": \"DevTools Protocol schema definition from the Microsoft Edge DevTools Protocol HTTP API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"object\",\n      \"description\": \"Protocol version\",\n      \"properties\": {\n        \"major\": {\n          \"type\": \"string\",\n          \"description\": \"Major version number\"\n        },\n        \"minor\": {\n          \"type\": \"string\",\n          \"description\": \"Minor version number\"\n        }\n      }\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"Protocol domains\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"domain\": {\n   \
  \         \"type\": \"string\",\n            \"description\": \"Domain name\"\n          },\n          \"experimental\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the domain is experimental\"\n          },\n          \"commands\": {\n            \"type\": \"array\",\n            \"description\": \"Domain commands\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Command name\"\n                },\n                \"parameters\": {\n                  \"type\": \"array\",\n                  \"description\": \"Command parameters\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"name\": {\n                        \"type\": \"string\"\n                      },\n                      \"type\": {\n              \
  \          \"type\": \"string\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          },\n          \"events\": {\n            \"type\": \"array\",\n            \"description\": \"Domain events\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/devtools-api-protocol-schema-schema.json
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
title: ProtocolSchema
---
