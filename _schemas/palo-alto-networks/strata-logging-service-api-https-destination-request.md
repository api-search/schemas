---
description: HTTPSDestinationRequest schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: HTTPSDestinationRequest
properties_list:
- description: Display name for this HTTPS destination.
  name: name
  type: string
- description: HTTPS endpoint URL.
  name: uri
  type: string
- description: ''
  name: http_method
  type: string
- description: Additional HTTP headers to include in log delivery requests.
  name: headers
  type: object
- description: ''
  name: tls_verify
  type: boolean
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-https-destination-request-schema.json
slug: strata-logging-service-api-https-destination-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HTTPSDestinationRequest\",\n  \"description\": \"HTTPSDestinationRequest schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-https-destination-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for this HTTPS destination.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS endpoint URL.\"\n    },\n    \"http_method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"PUT\"\n      ],\n      \"default\": \"POST\"\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Additional HTTP headers to include in log delivery requests.\",\n\
  \      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tls_verify\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"uri\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-https-destination-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: HTTPSDestinationRequest
---
