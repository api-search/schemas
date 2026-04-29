---
description: A USDA AMS market news report entry.
layout: schema
name: Report
properties_list:
- description: Unique identifier for the report.
  name: slug_id
  type: string
- description: Unique name for the report.
  name: slug_name
  type: string
- description: Date the report data covers.
  name: report_date
  type: string
- description: Date and time the report was published.
  name: published_date
  type: string
- description: Agricultural commodity covered by the report.
  name: commodity
  type: string
- description: Type of market covered (Weekly Summary, Daily, etc.).
  name: market_type
  type: string
- description: USDA AMS office that published the report.
  name: office
  type: string
- description: Section name within the report.
  name: section_name
  type: string
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-report-schema.json
slug: mars-api-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-report-schema.json\",\n  \"title\": \"Report\",\n  \"description\": \"A USDA AMS market news report entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"slug_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the report.\",\n      \"example\": \"2451\"\n    },\n    \"slug_name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the report.\",\n      \"example\": \"National Weekly Cattle Summary\"\n    },\n    \"report_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the report data covers.\",\n      \"example\": \"2026-04-18\"\n    },\n    \"published_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time\
  \ the report was published.\",\n      \"example\": \"2026-04-18T16:00:00Z\"\n    },\n    \"commodity\": {\n      \"type\": \"string\",\n      \"description\": \"Agricultural commodity covered by the report.\",\n      \"example\": \"Cattle\"\n    },\n    \"market_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of market covered (Weekly Summary, Daily, etc.).\",\n      \"example\": \"Weekly Summary\"\n    },\n    \"office\": {\n      \"type\": \"string\",\n      \"description\": \"USDA AMS office that published the report.\",\n      \"example\": \"National\"\n    },\n    \"section_name\": {\n      \"type\": \"string\",\n      \"description\": \"Section name within the report.\",\n      \"example\": \"All Classes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-report-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Report
---
