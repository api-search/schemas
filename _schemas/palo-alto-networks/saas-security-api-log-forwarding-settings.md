---
description: LogForwardingSettings schema from Palo Alto Networks SaaS Security API
layout: schema
name: LogForwardingSettings
properties_list:
- description: Whether log forwarding is globally enabled.
  name: enabled
  type: boolean
- description: ''
  name: destinations
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/saas-security-api-log-forwarding-settings-schema.json
slug: saas-security-api-log-forwarding-settings
source_filename: saas-security-api-log-forwarding-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogForwardingSettings\",\n  \"description\": \"LogForwardingSettings schema from Palo Alto Networks SaaS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-log-forwarding-settings-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether log forwarding is globally enabled.\"\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"syslog\",\n              \"https\",\n              \"s3\",\n              \"splunk\"\n            ],\n            \"description\": \"Forwarding destination type.\"\n          },\n          \"name\": {\n      \
  \      \"type\": \"string\",\n            \"description\": \"Destination name.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this destination is active.\"\n          },\n          \"log_types\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Log types forwarded to this destination.\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-log-forwarding-settings-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: LogForwardingSettings
---
