---
description: ''
layout: schema
name: GetAppointmentSlotsRequest
properties_list:
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: workTypeGroupId
  type: string
- description: ''
  name: workType
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: territoryIds
  type: string
- description: ''
  name: requiredResourceIds
  type: string
- description: ''
  name: schedulingPolicyId
  type: string
- description: ''
  name: allowConcurrentScheduling
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-appointment-slots-request-schema.json
slug: salesforce-get-appointment-slots-request
source_filename: salesforce-get-appointment-slots-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"startTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"workTypeGroupId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"workType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"territoryIds\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"requiredResourceIds\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"schedulingPolicyId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"allowConcurrentScheduling\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"startTime\"\
  ,\n    \"endTime\",\n    \"workTypeGroupId\",\n    \"workType\",\n    \"accountId\",\n    \"territoryIds\",\n    \"requiredResourceIds\",\n    \"schedulingPolicyId\",\n    \"allowConcurrentScheduling\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetAppointmentSlotsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-appointment-slots-request-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: GetAppointmentSlotsRequest
---
