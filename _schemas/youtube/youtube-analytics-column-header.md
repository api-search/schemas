---
description: Describes a single column in an Analytics report response, including its name, type, and data type.
layout: schema
name: ColumnHeader
properties_list:
- description: The name of the dimension or metric.
  name: name
  type: string
- description: The type of the column. Valid values are DIMENSION and METRIC.
  name: columnType
  type: string
- description: The type of data that the column contains. Valid values are STRING, INTEGER, FLOAT, and CURRENCY.
  name: dataType
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-analytics-column-header-schema.json
slug: youtube-analytics-column-header
source_filename: youtube-analytics-column-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a single column in an Analytics report response, including its name, type, and data type.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the dimension or metric.\",\n      \"example\": \"Example Title\"\n    },\n    \"columnType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the column. Valid values are DIMENSION and METRIC.\",\n      \"example\": \"DIMENSION\",\n      \"enum\": [\n        \"DIMENSION\",\n        \"METRIC\"\n      ]\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data that the column contains. Valid values are STRING, INTEGER, FLOAT, and CURRENCY.\",\n      \"example\": \"CURRENCY\",\n      \"enum\": [\n        \"CURRENCY\",\n        \"FLOAT\",\n        \"INTEGER\",\n        \"STRING\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ColumnHeader\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-analytics-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-analytics-column-header-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ColumnHeader
---
