---
description: ''
layout: schema
name: frequency
properties_list:
- description: 'String with frequency of a data series. Allowed values: - "D" (daily) - "W" (weekly) - "AW" (actual weekly) - "M" (monthly) - "AM" (actual monthly) - "Q" (quarterly) - "FQ" (fiscal quarterly) - "CQ" ('
  name: frequency
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-ownership-report-builder-frequency-schema.json
slug: factset-ownership-report-builder-frequency
source_filename: factset-ownership-report-builder-frequency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"frequency\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frequency\": {\n      \"type\": \"object\",\n      \"description\": \"String with frequency of a data series. Allowed values:\\n- \\\"D\\\" (daily)\\n- \\\"W\\\" (weekly)\\n- \\\"AW\\\" (actual weekly)\\n- \\\"M\\\" (monthly)\\n- \\\"AM\\\" (actual monthly)\\n- \\\"Q\\\" (quarterly)\\n- \\\"FQ\\\" (fiscal quarterly)\\n- \\\"CQ\\\" (calendar quarterly)\\n- \\\"AQ\\\" (actual quarterly)\\n- \\\"Y\\\" (yearly)\\n- \\\"FY\\\" (fiscal yearly)\\n- \\\"CY\\\" (calendar yearly)\\n- \\\"AY\\\" (actual yearly)\\n- \\\"MTD\\\" (month-to-date)\\n- \\\"QTD\\\" (quarter-to-date)\\n- \\\"YTD\\\" (year-to-date)\\n- \\\"FYTD\\\" (fiscal-year-to-date)\\n- \\\"CYTD\\\" (calendar-year-to-date)\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-ownership-report-builder-frequency-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: frequency
---
