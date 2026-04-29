---
description: 'A contiguous set of days: `startDate`, `startDate + 1`, ..., `endDate`. Requests are allowed up to 4 date ranges.'
layout: schema
name: DateRange
properties_list:
- description: 'The inclusive end date for the query in the format `YYYY-MM-DD`. Cannot be before `start_date`. The format `NdaysAgo`, `yesterday`, or `today` is also accepted, and in that case, the date is inferred '
  name: endDate
  type: string
- description: Assigns a name to this date range. The dimension `dateRange` is valued to this name in a report response. If set, cannot begin with `date_range_` or `RESERVED_`. If not set, date ranges are named by t
  name: name
  type: string
- description: The inclusive start date for the query in the format `YYYY-MM-DD`. Cannot be after `end_date`. The format `NdaysAgo`, `yesterday`, or `today` is also accepted, and in that case, the date is inferred b
  name: startDate
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-date-range-schema.json
slug: data-api-date-range
source_filename: data-api-date-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-date-range-schema.json\",\n  \"title\": \"DateRange\",\n  \"description\": \"A contiguous set of days: `startDate`, `startDate + 1`, ..., `endDate`. Requests are allowed up to 4 date ranges.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endDate\": {\n      \"description\": \"The inclusive end date for the query in the format `YYYY-MM-DD`. Cannot be before `start_date`. The format `NdaysAgo`, `yesterday`, or `today` is also accepted, and in that case, the date is inferred based on the property's reporting time zone.\",\n      \"type\": \"string\",\n      \"example\": \"2026-04-17\"\n    },\n    \"name\": {\n      \"description\": \"Assigns a name to this date range. The dimension `dateRange` is valued to this name in a report response. If set, cannot begin with `date_range_` or `RESERVED_`.\
  \ If not set, date ranges are named by their zero based index in the request: `date_range_0`, `date_range_1`, etc.\",\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"startDate\": {\n      \"description\": \"The inclusive start date for the query in the format `YYYY-MM-DD`. Cannot be after `end_date`. The format `NdaysAgo`, `yesterday`, or `today` is also accepted, and in that case, the date is inferred based on the property's reporting time zone.\",\n      \"type\": \"string\",\n      \"example\": \"2026-04-17\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-date-range-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: DateRange
---
