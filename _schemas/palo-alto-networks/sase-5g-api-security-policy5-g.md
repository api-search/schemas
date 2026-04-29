---
description: SecurityPolicy5G schema from Palo Alto Networks SASE 5G Managed Services API
layout: schema
name: SecurityPolicy5G
properties_list:
- description: Unique identifier of the security policy.
  name: policy_id
  type: string
- description: Display name of the security policy.
  name: name
  type: string
- description: Description of the policy's purpose.
  name: description
  type: string
- description: Whether threat prevention inspection is enabled.
  name: threat_prevention
  type: boolean
- description: Whether URL filtering is enabled for 5G data traffic.
  name: url_filtering
  type: boolean
- description: Whether application identification is enabled.
  name: app_identification
  type: boolean
- description: Whether SSL/TLS decryption is enabled.
  name: decryption
  type: boolean
- description: Whether log forwarding is enabled for this policy.
  name: log_forwarding
  type: boolean
- description: Whether this policy is active.
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-5g-api-security-policy5-g-schema.json
slug: sase-5g-api-security-policy5-g
source_filename: sase-5g-api-security-policy5-g-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SecurityPolicy5G\",\n  \"description\": \"SecurityPolicy5G schema from Palo Alto Networks SASE 5G Managed Services API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-security-policy5-g-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the security policy.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the security policy.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the policy's purpose.\"\n    },\n    \"threat_prevention\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether threat prevention inspection is enabled.\"\n    },\n    \"url_filtering\": {\n      \"type\": \"boolean\",\n   \
  \   \"description\": \"Whether URL filtering is enabled for 5G data traffic.\"\n    },\n    \"app_identification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether application identification is enabled.\"\n    },\n    \"decryption\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL/TLS decryption is enabled.\"\n    },\n    \"log_forwarding\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether log forwarding is enabled for this policy.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this policy is active.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-5g-api-security-policy5-g-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SecurityPolicy5G
---
