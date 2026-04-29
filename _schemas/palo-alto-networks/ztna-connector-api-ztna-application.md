---
description: ZTNAApplication schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: ZTNAApplication
properties_list:
- description: Unique identifier of the ZTNA application.
  name: app_id
  type: string
- description: Display name of the application.
  name: name
  type: string
- description: Description of the application.
  name: description
  type: string
- description: Connector group ID used to access this application.
  name: group_id
  type: string
- description: Fully qualified domain name of the private application.
  name: fqdn
  type: string
- description: TCP/UDP ports accessible through ZTNA.
  name: ports
  type: array
- description: Network protocols allowed for this application.
  name: protocols
  type: array
- description: Whether ZTNA access for this application is enabled.
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-ztna-application-schema.json
slug: ztna-connector-api-ztna-application
source_filename: ztna-connector-api-ztna-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZTNAApplication\",\n  \"description\": \"ZTNAApplication schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-ztna-application-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the ZTNA application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Connector group ID used to access this application.\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified\
  \ domain name of the private application.\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"TCP/UDP ports accessible through ZTNA.\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"TCP\",\n          \"UDP\"\n        ]\n      },\n      \"description\": \"Network protocols allowed for this application.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether ZTNA access for this application is enabled.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-ztna-application-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ZTNAApplication
---
