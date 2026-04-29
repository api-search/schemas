---
description: A security event report for a business site.
layout: schema
name: EventReport
properties_list:
- description: Site ID.
  name: siteId
  type: string
- description: Report time period.
  name: period
  type: object
- description: Summary statistics.
  name: summary
  type: object
- description: List of events in the period.
  name: events
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/business-api-event-report-schema.json
slug: business-api-event-report
source_filename: business-api-event-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-event-report-schema.json\",\n  \"title\": \"EventReport\",\n  \"description\": \"A security event report for a business site.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"Site ID.\",\n      \"example\": \"site-001\"\n    },\n    \"period\": {\n      \"type\": \"object\",\n      \"description\": \"Report time period.\",\n      \"properties\": {\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"summary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary statistics.\",\n      \"properties\": {\n        \"totalAlarms\": {\n     \
  \     \"type\": \"integer\",\n          \"description\": \"Total alarm events.\",\n          \"example\": 2\n        },\n        \"totalAccessEvents\": {\n          \"type\": \"integer\",\n          \"description\": \"Total access control events.\",\n          \"example\": 150\n        }\n      }\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"List of events in the period.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-event-report-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: EventReport
---
