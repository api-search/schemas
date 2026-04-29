---
description: Definition of an analytics report request
layout: schema
name: ReportRequest
properties_list:
- description: The report suite ID to run the report against
  name: rsid
  type: string
- description: Locale for response labels
  name: locale
  type: string
- description: List of global filters applied to the entire report
  name: globalFilters
  type: array
- description: Container defining the metrics to include in a report
  name: metricContainer
  type: object
- description: The primary dimension ID for the report (e.g. variables/page)
  name: dimension
  type: string
- description: Settings that control report output behavior
  name: settings
  type: object
- description: Statistical settings for the report
  name: statistics
  type: object
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-request-schema.json
slug: adobe-analytics-report-request
source_filename: adobe-analytics-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Definition of an analytics report request\",\n  \"properties\": {\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"The report suite ID to run the report against\",\n      \"example\": \"examplersid\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"Locale for response labels\",\n      \"example\": \"en_US\"\n    },\n    \"globalFilters\": {\n      \"type\": \"array\",\n      \"description\": \"List of global filters applied to the entire report\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A filter applied to a report\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Filter type\",\n            \"example\": \"dateRange\",\n            \"enum\": [\n              \"dateRange\",\n              \"breakdown\",\n              \"segment\"\n         \
  \   ]\n          },\n          \"dateRange\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 date range (e.g. 2024-01-01T00:00:00/2024-01-31T23:59:59)\",\n            \"example\": \"example_value\"\n          },\n          \"segmentId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of an existing segment to apply as a filter\",\n            \"example\": \"500123\"\n          },\n          \"dimension\": {\n            \"type\": \"string\",\n            \"description\": \"Dimension for breakdown filter\",\n            \"example\": \"example_value\"\n          },\n          \"itemId\": {\n            \"type\": \"string\",\n            \"description\": \"Dimension item ID for breakdown filter\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"type\"\n        ]\n      }\n    },\n    \"metricContainer\": {\n      \"type\": \"object\",\n      \"description\": \"Container defining the\
  \ metrics to include in a report\",\n      \"properties\": {\n        \"metrics\": {\n          \"type\": \"array\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"description\": \"A metric included in a report request\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The metric ID (e.g. metrics/visits)\",\n                \"example\": \"abc123\"\n              },\n              \"columnId\": {\n                \"type\": \"string\",\n                \"description\": \"Column identifier for this metric in the response\",\n                \"example\": \"500123\"\n              },\n              \"filters\": {\n                \"type\": \"array\",\n                \"description\": \"Metric-level filter IDs referencing metricFilters\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"string\"\n             \
  \   }\n              },\n              \"sort\": {\n                \"type\": \"string\",\n                \"description\": \"Sort direction for this metric\",\n                \"example\": \"ASC\",\n                \"enum\": [\n                  \"ASC\",\n                  \"DESC\"\n                ]\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          }\n        },\n        \"metricFilters\": {\n          \"type\": \"array\",\n          \"description\": \"Filters applied at the metric level\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"description\": \"A filter applied to a report\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Filter type\",\n                \"example\": \"dateRange\",\n                \"enum\": [\n                  \"dateRange\",\n                  \"breakdown\",\n\
  \                  \"segment\"\n                ]\n              },\n              \"dateRange\": {\n                \"type\": \"string\",\n                \"description\": \"ISO 8601 date range (e.g. 2024-01-01T00:00:00/2024-01-31T23:59:59)\",\n                \"example\": \"example_value\"\n              },\n              \"segmentId\": {\n                \"type\": \"string\",\n                \"description\": \"ID of an existing segment to apply as a filter\",\n                \"example\": \"500123\"\n              },\n              \"dimension\": {\n                \"type\": \"string\",\n                \"description\": \"Dimension for breakdown filter\",\n                \"example\": \"example_value\"\n              },\n              \"itemId\": {\n                \"type\": \"string\",\n                \"description\": \"Dimension item ID for breakdown filter\",\n                \"example\": \"500123\"\n              }\n            },\n            \"required\": [\n              \"\
  type\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"metrics\"\n      ]\n    },\n    \"dimension\": {\n      \"type\": \"string\",\n      \"description\": \"The primary dimension ID for the report (e.g. variables/page)\",\n      \"example\": \"variables/page\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Settings that control report output behavior\",\n      \"properties\": {\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of rows to return\",\n          \"example\": 10\n        },\n        \"page\": {\n          \"type\": \"integer\",\n          \"description\": \"Page number (zero-indexed)\",\n          \"example\": 10\n        },\n        \"nonesBehavior\": {\n          \"type\": \"string\",\n          \"description\": \"How to handle None values\",\n          \"example\": \"exclude-nones\",\n          \"enum\": [\n            \"exclude-nones\",\n        \
  \    \"return-nones\"\n          ]\n        }\n      }\n    },\n    \"statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Statistical settings for the report\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"rsid\",\n    \"globalFilters\",\n    \"metricContainer\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-request-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportRequest
---
