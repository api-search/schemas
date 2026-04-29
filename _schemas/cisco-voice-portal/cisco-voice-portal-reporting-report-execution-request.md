---
description: ''
layout: schema
name: ReportExecutionRequest
properties_list:
- description: Report parameters as defined by the template
  name: parameters
  type: object
- description: ''
  name: format
  type: string
- description: Whether to execute asynchronously
  name: async
  type: boolean
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-report-execution-request-schema.json
slug: cisco-voice-portal-reporting-report-execution-request
source_filename: cisco-voice-portal-reporting-report-execution-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportExecutionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Report parameters as defined by the template\"\n    },\n    \"format\": {\n      \"type\": \"string\"\n    },\n    \"async\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to execute asynchronously\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-report-execution-request-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ReportExecutionRequest
---
