---
description: Date range configuration for reports.
layout: schema
name: DateRange
properties_list:
- description: The start date of the date range, inclusive. Format is YYYY-MM-DD.
  name: startDate
  type: string
- description: The end date of the date range, inclusive. Format is YYYY-MM-DD.
  name: endDate
  type: string
- description: The date range relative to the date of when the report is run.
  name: relativeDateRange
  type: string
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-date-range-schema.json
slug: google-campaign-manager-date-range
source_filename: google-campaign-manager-date-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DateRange\",\n  \"type\": \"object\",\n  \"description\": \"Date range configuration for reports.\",\n  \"properties\": {\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the date range, inclusive. Format is YYYY-MM-DD.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The end date of the date range, inclusive. Format is YYYY-MM-DD.\"\n    },\n    \"relativeDateRange\": {\n      \"type\": \"string\",\n      \"description\": \"The date range relative to the date of when the report is run.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-date-range-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: DateRange
---
