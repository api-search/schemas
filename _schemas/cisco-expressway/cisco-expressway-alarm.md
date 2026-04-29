---
description: 'Schema for an alarm on Cisco Expressway. Alarms indicate events or configuration changes that require administrator intervention, or hardware and environmental issues. Alarm IDs are grouped by prefix ranges: 10nnn hardware, 15nnn software, 20nnn cluster, 25nnn network, 30nnn licensing, 35nnn external services, 40nnn security, 45nnn configuration, 55nnn B2BUA, 6xxxx hybrid services, 9xxxx operational events.'
layout: schema
name: Cisco Expressway Alarm
properties_list:
- description: 'Unique alarm identifier. The prefix range indicates the alarm category: 10nnn for hardware failures, 15nnn for software issues, 20nnn for cluster problems, 25nnn for network configuration, 30nnn for l'
  name: AlarmId
  type: string
- description: Severity level of the alarm indicating the urgency of required action
  name: Severity
  type: string
- description: Short description of the alarm condition
  name: Title
  type: string
- description: Detailed explanation of the alarm condition and suggested remediation action
  name: Description
  type: string
- description: ISO 8601 timestamp when the alarm was raised
  name: TimeRaised
  type: string
- description: Category of the alarm based on the alarm ID prefix range
  name: Category
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-alarm-schema.json
slug: cisco-expressway-alarm
source_filename: cisco-expressway-alarm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-alarm-schema.json\",\n  \"title\": \"Cisco Expressway Alarm\",\n  \"description\": \"Schema for an alarm on Cisco Expressway. Alarms indicate events or configuration changes that require administrator intervention, or hardware and environmental issues. Alarm IDs are grouped by prefix ranges: 10nnn hardware, 15nnn software, 20nnn cluster, 25nnn network, 30nnn licensing, 35nnn external services, 40nnn security, 45nnn configuration, 55nnn B2BUA, 6xxxx hybrid services, 9xxxx operational events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique alarm identifier. The prefix range indicates the alarm category: 10nnn for hardware failures, 15nnn for software issues, 20nnn for cluster problems, 25nnn for network configuration, 30nnn for licensing,\
  \ 35nnn for external service failures, 40nnn for security, 45nnn for configuration anomalies, 55nnn for B2BUA errors, 6xxxx for hybrid services, 9xxxx for significant operational events.\",\n      \"pattern\": \"^\\\\d{5,6}$\",\n      \"examples\": [\"10001\", \"30001\", \"40001\"]\n    },\n    \"Severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the alarm indicating the urgency of required action\",\n      \"enum\": [\"Critical\", \"Warning\", \"Information\"]\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the alarm condition\",\n      \"examples\": [\"License capacity exceeded\", \"Certificate expiring\", \"Cluster communication failure\"]\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed explanation of the alarm condition and suggested remediation action\"\n    },\n    \"TimeRaised\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"ISO 8601 timestamp when the alarm was raised\"\n    },\n    \"Category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the alarm based on the alarm ID prefix range\",\n      \"enum\": [\n        \"Hardware\",\n        \"Software\",\n        \"Cluster\",\n        \"Network\",\n        \"Licensing\",\n        \"External Services\",\n        \"Security\",\n        \"Configuration\",\n        \"B2BUA\",\n        \"Hybrid Services\",\n        \"Operational\"\n      ]\n    }\n  },\n  \"required\": [\"AlarmId\", \"Severity\", \"Title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-alarm-schema.json
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Alarm
---
