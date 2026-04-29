---
description: EmailDestination schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: EmailDestination
properties_list:
- description: Unique identifier of the email destination.
  name: destination_id
  type: string
- description: Display name of the destination.
  name: name
  type: string
- description: SMTP server hostname.
  name: gateway
  type: string
- description: Sender email address.
  name: from
  type: string
- description: Recipient email address.
  name: to
  type: string
- description: Additional recipient email address.
  name: and_also_to
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-email-destination-schema.json
slug: strata-logging-service-api-email-destination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailDestination\",\n  \"description\": \"EmailDestination schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-email-destination-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the email destination.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the destination.\"\n    },\n    \"gateway\": {\n      \"type\": \"string\",\n      \"description\": \"SMTP server hostname.\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Sender email address.\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n\
  \      \"description\": \"Recipient email address.\"\n    },\n    \"and_also_to\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Additional recipient email address.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-email-destination-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailDestination
---
