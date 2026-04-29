---
description: ''
layout: schema
name: ReportResult
properties_list:
- description: ''
  name: reportId
  type: string
- description: ''
  name: templateId
  type: string
- description: ''
  name: templateName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: generatedAt
  type: string
- description: ''
  name: parameters
  type: object
- description: ''
  name: columns
  type: array
- description: ''
  name: rows
  type: array
- description: ''
  name: totalRows
  type: integer
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-report-result-schema.json
slug: cisco-voice-portal-reporting-report-result
source_filename: cisco-voice-portal-reporting-report-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"type\": \"string\"\n    },\n    \"templateId\": {\n      \"type\": \"string\"\n    },\n    \"templateName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"generatedAt\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"object\"\n    },\n    \"columns\": {\n      \"type\": \"array\"\n    },\n    \"rows\": {\n      \"type\": \"array\"\n    },\n    \"totalRows\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-report-result-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ReportResult
---
