---
description: Represents a security event detected by the Trellix Web Gateway, including malware detections, phishing attempts, policy violations, and data loss prevention triggers.
layout: schema
name: Trellix Web Gateway Security Event
properties_list:
- description: Unique identifier for the security event
  name: id
  type: string
- description: Time the security event occurred
  name: timestamp
  type: string
- description: Severity level of the security event
  name: severity
  type: string
- description: Type of security event detected
  name: eventType
  type: string
- description: IP address of the client that triggered the event
  name: sourceIp
  type: string
- description: Authenticated user name associated with the event
  name: user
  type: string
- description: URL involved in the security event
  name: url
  type: string
- description: Name of the detected threat or malware
  name: threatName
  type: string
- description: Action taken by the gateway in response to the event
  name: action
  type: string
- description: Name of the policy rule that triggered the event
  name: ruleName
  type: string
- description: Additional descriptive details about the event
  name: details
  type: string
provider_name: Trellix Web Gateway
provider_slug: trellix-web-gateway
schema_file: json-schema/trellix-web-gateway-security-event-schema.json
slug: trellix-web-gateway-security-event
source_filename: trellix-web-gateway-security-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.trellix.com/schemas/web-gateway/security-event.json\",\n  \"title\": \"Trellix Web Gateway Security Event\",\n  \"description\": \"Represents a security event detected by the Trellix Web Gateway, including malware detections, phishing attempts, policy violations, and data loss prevention triggers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the security event\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the security event occurred\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"medium\", \"high\", \"critical\"],\n      \"description\": \"Severity level of the security event\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"malware\"\
  ,\n        \"phishing\",\n        \"policy_violation\",\n        \"data_leak\",\n        \"certificate_error\",\n        \"authentication_failure\"\n      ],\n      \"description\": \"Type of security event detected\"\n    },\n    \"sourceIp\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the client that triggered the event\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Authenticated user name associated with the event\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL involved in the security event\"\n    },\n    \"threatName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the detected threat or malware\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\"blocked\", \"quarantined\", \"logged\", \"cleaned\"],\n      \"description\": \"Action taken by the gateway in response to the event\"\n    },\n    \"ruleName\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Name of the policy rule that triggered the event\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional descriptive details about the event\"\n    }\n  },\n  \"required\": [\"id\", \"timestamp\", \"severity\", \"eventType\", \"action\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/trellix-web-gateway/refs/heads/main/json-schema/trellix-web-gateway-security-event-schema.json
tags:
- Cybersecurity
- Data Loss Prevention
- Enterprise Security
- Malware Protection
- Network Security
- Threat Protection
- URL Filtering
- Web Gateway
title: Trellix Web Gateway Security Event
---
