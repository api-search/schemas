---
description: HTTPSDestination schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: HTTPSDestination
properties_list:
- description: Unique identifier of the HTTPS destination.
  name: destination_id
  type: string
- description: Display name of the destination.
  name: name
  type: string
- description: HTTPS endpoint URL where logs are posted.
  name: uri
  type: string
- description: HTTP method used to deliver logs.
  name: http_method
  type: string
- description: Whether TLS certificate verification is enabled.
  name: tls_verify
  type: boolean
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-https-destination-schema.json
slug: strata-logging-service-api-https-destination
source_filename: strata-logging-service-api-https-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HTTPSDestination\",\n  \"description\": \"HTTPSDestination schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-https-destination-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the HTTPS destination.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the destination.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS endpoint URL where logs are posted.\"\n    },\n    \"http_method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"PUT\"\n      ],\n      \"description\": \"HTTP method used to deliver\
  \ logs.\"\n    },\n    \"tls_verify\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether TLS certificate verification is enabled.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-https-destination-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: HTTPSDestination
---
