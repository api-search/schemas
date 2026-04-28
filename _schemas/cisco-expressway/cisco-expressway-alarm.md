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
