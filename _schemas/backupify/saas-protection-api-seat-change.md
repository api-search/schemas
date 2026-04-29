---
description: A single seat change action
layout: schema
name: SeatChange
properties_list:
- description: Remote identifier for the seat
  name: remoteId
  type: string
- description: Action to perform on the seat
  name: action
  type: string
- description: Type of seat
  name: seatType
  type: string
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-seat-change-schema.json
slug: saas-protection-api-seat-change
source_filename: saas-protection-api-seat-change-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seat-change-schema.json\",\n  \"title\": \"SeatChange\",\n  \"description\": \"A single seat change action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"remoteId\": {\n      \"type\": \"string\",\n      \"description\": \"Remote identifier for the seat\",\n      \"example\": \"user-abc123\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"License\",\n        \"Unlicense\",\n        \"Pause\"\n      ],\n      \"description\": \"Action to perform on the seat\",\n      \"example\": \"License\"\n    },\n    \"seatType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"User\",\n        \"SharedMailbox\",\n        \"Site\",\n        \"TeamSite\",\n        \"Team\"\n      ],\n      \"description\": \"Type of seat\",\n      \"example\":\
  \ \"User\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seat-change-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: SeatChange
---
