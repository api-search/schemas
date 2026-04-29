---
description: A licensed or unlicensed seat (user, mailbox, site, or team)
layout: schema
name: Seat
properties_list:
- description: Remote identifier for the seat in the source system
  name: remoteId
  type: string
- description: Display name of the seat
  name: displayName
  type: string
- description: Email address for user seats
  name: email
  type: string
- description: Type of seat
  name: seatType
  type: string
- description: Current license status
  name: licenseStatus
  type: string
- description: Timestamp of last successful backup
  name: lastBackup
  type: string
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-seat-schema.json
slug: saas-protection-api-seat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seat-schema.json\",\n  \"title\": \"Seat\",\n  \"description\": \"A licensed or unlicensed seat (user, mailbox, site, or team)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"remoteId\": {\n      \"type\": \"string\",\n      \"description\": \"Remote identifier for the seat in the source system\",\n      \"example\": \"user-abc123\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the seat\",\n      \"example\": \"John Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address for user seats\",\n      \"example\": \"jsmith@company.com\"\n    },\n    \"seatType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"User\",\n        \"SharedMailbox\"\
  ,\n        \"Site\",\n        \"TeamSite\",\n        \"Team\"\n      ],\n      \"description\": \"Type of seat\",\n      \"example\": \"User\"\n    },\n    \"licenseStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Licensed\",\n        \"Unlicensed\",\n        \"Paused\"\n      ],\n      \"description\": \"Current license status\",\n      \"example\": \"Licensed\"\n    },\n    \"lastBackup\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last successful backup\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seat-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: Seat
---
