---
description: Detailed commodity price and market data from a report.
layout: schema
name: Report Data
properties_list:
- description: Unique identifier for the report.
  name: slug_id
  type: string
- description: Name of the report.
  name: slug_name
  type: string
- description: Date the report data covers.
  name: report_date
  type: string
- description: Date the report was published.
  name: published_date
  type: string
- description: Agricultural commodity.
  name: commodity
  type: string
- description: Class or category within the commodity.
  name: class
  type: string
- description: Grade or quality designation.
  name: grade
  type: string
- description: Number of head (animals) in the report.
  name: head_count
  type: integer
- description: Price per hundredweight (CWT).
  name: price_per_cwt
  type: number
- description: Unit of price measurement.
  name: price_unit
  type: string
- description: Geographic region covered.
  name: region
  type: string
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
schema_file: json-schema/mars-api-report-data-schema.json
slug: mars-api-report-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-report-data-schema.json\",\n  \"title\": \"Report Data\",\n  \"description\": \"Detailed commodity price and market data from a report.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"slug_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the report.\",\n      \"example\": \"2451\"\n    },\n    \"slug_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the report.\",\n      \"example\": \"National Weekly Cattle Summary\"\n    },\n    \"report_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the report data covers.\",\n      \"example\": \"2026-04-18\"\n    },\n    \"published_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Date the report was published.\",\n      \"example\": \"2026-04-18T16:00:00Z\"\n    },\n    \"commodity\": {\n      \"type\": \"string\",\n      \"description\": \"Agricultural commodity.\",\n      \"example\": \"Cattle\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"Class or category within the commodity.\",\n      \"example\": \"Slaughter\"\n    },\n    \"grade\": {\n      \"type\": \"string\",\n      \"description\": \"Grade or quality designation.\",\n      \"example\": \"Choice\"\n    },\n    \"head_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of head (animals) in the report.\",\n      \"example\": 45000\n    },\n    \"price_per_cwt\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Price per hundredweight (CWT).\",\n      \"example\": 185.5\n    },\n    \"price_unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of price measurement.\",\n      \"example\"\
  : \"CWT\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic region covered.\",\n      \"example\": \"National\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/json-schema/mars-api-report-data-schema.json
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
title: Report Data
---
