---
description: SecurityPolicy5GRequest schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: SecurityPolicy5GRequest
properties_list:
- description: Display name for the security policy.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: ''
  name: threat_prevention
  type: boolean
- description: ''
  name: url_filtering
  type: boolean
- description: ''
  name: app_identification
  type: boolean
- description: ''
  name: decryption
  type: boolean
- description: ''
  name: log_forwarding
  type: boolean
- description: ''
  name: enabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-security-policy5-g-request-schema.json
slug: sase-5g-api-security-policy5-g-request
source_filename: sase-5g-api-security-policy5-g-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityPolicy5GRequest\",\n  \"description\": \"SecurityPolicy5GRequest schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-security-policy5-g-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the security policy.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"threat_prevention\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"url_filtering\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"app_identification\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"decryption\": {\n      \"type\": \"boolean\"\
  ,\n      \"default\": false\n    },\n    \"log_forwarding\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-security-policy5-g-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SecurityPolicy5GRequest
---
