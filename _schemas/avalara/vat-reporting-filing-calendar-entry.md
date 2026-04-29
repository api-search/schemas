---
description: FilingCalendarEntry schema from Avalara API
layout: schema
name: FilingCalendarEntry
properties_list:
- description: ''
  name: countryCode
  type: string
- description: ''
  name: returnType
  type: string
- description: ''
  name: filingFrequency
  type: string
- description: ''
  name: periodStart
  type: string
- description: ''
  name: periodEnd
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: status
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/vat-reporting-filing-calendar-entry-schema.json
slug: vat-reporting-filing-calendar-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-filing-calendar-entry-schema.json\",\n  \"title\": \"FilingCalendarEntry\",\n  \"description\": \"FilingCalendarEntry schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countryCode\": {\n      \"type\": \"string\"\n    },\n    \"returnType\": {\n      \"type\": \"string\"\n    },\n    \"filingFrequency\": {\n      \"type\": \"string\"\n    },\n    \"periodStart\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"periodEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Upcoming\",\n        \"Due\",\n        \"Overdue\",\n        \"Filed\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/vat-reporting-filing-calendar-entry-schema.json
tags:
- Taxes
title: FilingCalendarEntry
---
