---
description: ''
layout: schema
name: PayGroupDetail
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: payPeriodStartDate
  type: string
- description: ''
  name: payPeriodEndDate
  type: string
- description: ''
  name: payDate
  type: string
- description: ''
  name: payRunStatus
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/payroll-pay-group-detail-schema.json
slug: payroll-pay-group-detail
source_filename: payroll-pay-group-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PayGroupDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"payPeriodStartDate\": {\n      \"type\": \"string\"\n    },\n    \"payPeriodEndDate\": {\n      \"type\": \"string\"\n    },\n    \"payDate\": {\n      \"type\": \"string\"\n    },\n    \"payRunStatus\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/payroll-pay-group-detail-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: PayGroupDetail
---
