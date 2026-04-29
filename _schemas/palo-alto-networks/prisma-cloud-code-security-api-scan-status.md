---
description: ScanStatus schema from Palo Alto Networks Prisma Cloud Code Security API
layout: schema
name: ScanStatus
properties_list:
- description: Unique scan identifier.
  name: scan_id
  type: string
- description: Repository that was scanned.
  name: repositoryId
  type: string
- description: Branch that was scanned.
  name: branch
  type: string
- description: Current scan status.
  name: status
  type: string
- description: Scan start timestamp.
  name: startTime
  type: string
- description: Scan completion timestamp.
  name: endTime
  type: string
- description: Types of scans included in this run.
  name: scanTypes
  type: array
- description: High-level scan result summary. Available after completion.
  name: summary
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-code-security-api-scan-status-schema.json
slug: prisma-cloud-code-security-api-scan-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScanStatus\",\n  \"description\": \"ScanStatus schema from Palo Alto Networks Prisma Cloud Code Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-scan-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scan_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique scan identifier.\"\n    },\n    \"repositoryId\": {\n      \"type\": \"string\",\n      \"description\": \"Repository that was scanned.\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Branch that was scanned.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"queued\",\n        \"running\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Current scan status.\"\n    },\n    \"startTime\":\
  \ {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scan start timestamp.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scan completion timestamp.\"\n    },\n    \"scanTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"iac\",\n          \"sca\",\n          \"secrets\",\n          \"cicd\"\n        ]\n      },\n      \"description\": \"Types of scans included in this run.\"\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"description\": \"High-level scan result summary. Available after completion.\",\n      \"properties\": {\n        \"filesScanned\": {\n          \"type\": \"integer\"\n        },\n        \"resourcesScanned\": {\n          \"type\": \"integer\"\n        },\n        \"errorsBySeverity\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"critical\"\
  : {\n              \"type\": \"integer\"\n            },\n            \"high\": {\n              \"type\": \"integer\"\n            },\n            \"medium\": {\n              \"type\": \"integer\"\n            },\n            \"low\": {\n              \"type\": \"integer\"\n            },\n            \"info\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-scan-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ScanStatus
---
