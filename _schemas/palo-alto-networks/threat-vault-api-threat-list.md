---
description: ThreatList schema from Palo Alto Networks Threat Vault API
layout: schema
name: ThreatList
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
- description: Total number of matching signatures.
  name: count
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/threat-vault-api-threat-list-schema.json
slug: threat-vault-api-threat-list
source_filename: threat-vault-api-threat-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ThreatList\",\n  \"description\": \"ThreatList schema from Palo Alto Networks Threat Vault API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-threat-list-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"zingbox\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"description\": \"Threat signature metadata record.\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\",\n                \"description\": \"Unique signature identifier.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Signature name.\"\
  \n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"antivirus\",\n                  \"antispyware\",\n                  \"vulnerability\",\n                  \"dns\",\n                  \"fileformat\"\n                ],\n                \"description\": \"Signature type category.\"\n              },\n              \"subtype\": {\n                \"type\": \"string\",\n                \"description\": \"Signature subtype (e.g., virus, trojan, exploit).\"\n              },\n              \"severity\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"critical\",\n                  \"high\",\n                  \"medium\",\n                  \"low\",\n                  \"informational\"\n                ]\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"Human-readable description of the threat.\"\
  \n              },\n              \"cve\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"description\": \"Associated CVE identifiers.\"\n              },\n              \"default_action\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"alert\",\n                  \"allow\",\n                  \"drop\",\n                  \"reset-both\",\n                  \"reset-client\",\n                  \"reset-server\",\n                  \"block-ip\",\n                  \"sinkhole\"\n                ],\n                \"description\": \"Default action applied to traffic matching this signature.\"\n              },\n              \"min_version\": {\n                \"type\": \"string\",\n                \"description\": \"Minimum PAN-OS version supporting this signature.\"\n              },\n              \"max_version\": {\n                \"type\":\
  \ \"string\",\n                \"description\": \"Maximum PAN-OS version supporting this signature (empty if still active).\"\n              },\n              \"status\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"released\",\n                  \"deprecated\",\n                  \"disabled\"\n                ]\n              },\n              \"ori_release_version\": {\n                \"type\": \"string\",\n                \"description\": \"Content version in which this signature was first released.\"\n              },\n              \"latest_release_version\": {\n                \"type\": \"string\",\n                \"description\": \"Most recent content version that updated this signature.\"\n              },\n              \"first_release_time\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Timestamp when the signature was first released.\"\n              },\n\
  \              \"latest_release_time\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\",\n                \"description\": \"Timestamp of the most recent signature update.\"\n              },\n              \"sha256\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"description\": \"SHA-256 hashes associated with this signature (antivirus).\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching signatures.\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-threat-list-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ThreatList
---
