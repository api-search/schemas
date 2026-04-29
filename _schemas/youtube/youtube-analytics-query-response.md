---
description: Response to a successful YouTube Analytics query request containing the requested report data including column headers and rows of data.
layout: schema
name: QueryResponse
properties_list:
- description: Identifies the API resource's type. Value is youtubeAnalytics#resultTable.
  name: kind
  type: string
- description: A list of objects that describe the columns in the report table. Each object in the list identifies a query dimension or metric and provides information about the data type of that dimension or metric
  name: columnHeaders
  type: array
- description: The list contains all rows of the result table. Each item in the list is an array that contains comma-delimited data corresponding to a single row of data. The order of the comma-delimited data fields
  name: rows
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-analytics-query-response-schema.json
slug: youtube-analytics-query-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response to a successful YouTube Analytics query request containing the requested report data including column headers and rows of data.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtubeAnalytics#resultTable.\",\n      \"example\": \"youtube#video\"\n    },\n    \"columnHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"A list of objects that describe the columns in the report table. Each object in the list identifies a query dimension or metric and provides information about the data type of that dimension or metric.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Describes a single column in an Analytics report response, including its name, type, and data type.\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n    \
  \        \"description\": \"The name of the dimension or metric.\",\n            \"example\": \"Example Title\"\n          },\n          \"columnType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of the column. Valid values are DIMENSION and METRIC.\",\n            \"example\": \"DIMENSION\",\n            \"enum\": [\n              \"DIMENSION\",\n              \"METRIC\"\n            ]\n          },\n          \"dataType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of data that the column contains. Valid values are STRING, INTEGER, FLOAT, and CURRENCY.\",\n            \"example\": \"CURRENCY\",\n            \"enum\": [\n              \"CURRENCY\",\n              \"FLOAT\",\n              \"INTEGER\",\n              \"STRING\"\n            ]\n          }\n        }\n      }\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"The list contains all rows of the result table. Each item in the\
  \ list is an array that contains comma-delimited data corresponding to a single row of data. The order of the comma-delimited data fields will match the order of the columns listed in the columnHeaders field.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"array\",\n        \"description\": \"A single row of data in the report result set.\",\n        \"items\": {\n          \"type\": \"object\",\n          \"description\": \"A value in the row, either a string or number depending on the column type.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-analytics-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-analytics-query-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: QueryResponse
---
