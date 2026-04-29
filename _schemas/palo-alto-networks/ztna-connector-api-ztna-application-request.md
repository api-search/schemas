---
description: ZTNAApplicationRequest schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: ZTNAApplicationRequest
properties_list:
- description: Display name for the ZTNA application.
  name: name
  type: string
- description: Optional description of the application.
  name: description
  type: string
- description: Connector group ID to use for accessing the application.
  name: group_id
  type: string
- description: Fully qualified domain name of the private application.
  name: fqdn
  type: string
- description: TCP/UDP ports to expose through ZTNA.
  name: ports
  type: array
- description: Network protocols to allow.
  name: protocols
  type: array
- description: Whether to enable ZTNA access immediately after creation.
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-ztna-application-request-schema.json
slug: ztna-connector-api-ztna-application-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZTNAApplicationRequest\",\n  \"description\": \"ZTNAApplicationRequest schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-ztna-application-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the ZTNA application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the application.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Connector group ID to use for accessing the application.\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified domain name of the private application.\"\n    },\n    \"ports\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"TCP/UDP ports to expose through ZTNA.\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"TCP\",\n          \"UDP\"\n        ]\n      },\n      \"description\": \"Network protocols to allow.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether to enable ZTNA access immediately after creation.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"group_id\",\n    \"fqdn\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-ztna-application-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ZTNAApplicationRequest
---
