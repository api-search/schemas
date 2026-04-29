---
description: Usage report configuration
layout: schema
name: Report
properties_list:
- description: Report identifier
  name: id
  type: string
- description: Report schedule configuration
  name: schedule
  type: object
- description: Report parameters
  name: parameters
  type: object
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-report-schema.json
slug: account-management-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-report-schema.json\",\n  \"title\": \"Report\",\n  \"description\": \"Usage report configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Report identifier\"\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Report schedule configuration\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Report parameters\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-report-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Report
---
