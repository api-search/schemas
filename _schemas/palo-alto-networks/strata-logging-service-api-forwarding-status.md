---
description: ForwardingStatus schema from Palo Alto Networks Strata Logging Service API
layout: schema
name: ForwardingStatus
properties_list:
- description: Log forwarding profile identifier.
  name: profile_id
  type: string
- description: Overall health status of the forwarding profile.
  name: overall_status
  type: string
- description: Per-destination status details.
  name: destinations
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-service-api-forwarding-status-schema.json
slug: strata-logging-service-api-forwarding-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForwardingStatus\",\n  \"description\": \"ForwardingStatus schema from Palo Alto Networks Strata Logging Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-forwarding-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profile_id\": {\n      \"type\": \"string\",\n      \"description\": \"Log forwarding profile identifier.\"\n    },\n    \"overall_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"healthy\",\n        \"degraded\",\n        \"error\"\n      ],\n      \"description\": \"Overall health status of the forwarding profile.\"\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"description\": \"Per-destination status details.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"destination_id\"\
  : {\n            \"type\": \"string\"\n          },\n          \"destination_type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"syslog\",\n              \"https\",\n              \"email\"\n            ]\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"healthy\",\n              \"error\",\n              \"disabled\"\n            ]\n          },\n          \"last_successful_delivery\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"error_count_24h\": {\n            \"type\": \"integer\"\n          },\n          \"last_error\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-service-api-forwarding-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ForwardingStatus
---
