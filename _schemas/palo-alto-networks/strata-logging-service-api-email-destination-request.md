---
description: EmailDestinationRequest schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: EmailDestinationRequest
properties_list:
- description: Display name for this email destination.
  name: name
  type: string
- description: SMTP server hostname or IP address.
  name: gateway
  type: string
- description: Sender email address.
  name: from
  type: string
- description: Primary recipient email address.
  name: to
  type: string
- description: Additional recipient email address.
  name: and_also_to
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-email-destination-request-schema.json
slug: strata-logging-service-api-email-destination-request
source_filename: strata-logging-service-api-email-destination-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailDestinationRequest\",\n  \"description\": \"EmailDestinationRequest schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-email-destination-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for this email destination.\"\n    },\n    \"gateway\": {\n      \"type\": \"string\",\n      \"description\": \"SMTP server hostname or IP address.\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Sender email address.\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary recipient email address.\"\n    },\n    \"and_also_to\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Additional recipient email address.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"gateway\",\n    \"from\",\n    \"to\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-email-destination-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailDestinationRequest
---
