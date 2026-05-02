---
description: Represents a Looker Studio data source, which defines a connection to an underlying data set and its field schema. Data sources can be reusable (shared across reports) or embedded within a specific report.
layout: schema
name: Looker Studio Data Source
properties_list:
- description: The resource name of the data source, serving as its unique identifier.
  name: name
  type: string
- description: The display title of the data source.
  name: title
  type: string
- description: The email address of the data source owner.
  name: owner
  type: string
- description: The email address of the user who created the data source.
  name: creator
  type: string
- description: The timestamp when the data source was created.
  name: createTime
  type: string
- description: The timestamp when the data source was last modified.
  name: updateTime
  type: string
- description: Whether the data source has been moved to the trash.
  name: trashed
  type: boolean
- description: The type of connector used by this data source.
  name: connectorType
  type: string
- description: The field definitions that make up the data source schema.
  name: fields
  type: array
provider_name: Looker Studio
provider_slug: looker-studio
schema_file: json-schema/looker-studio-data-source-schema.json
slug: looker-studio-data-source
source_filename: looker-studio-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/looker-studio/json-schema/looker-studio-data-source-schema.json\",\n  \"title\": \"Looker Studio Data Source\",\n  \"description\": \"Represents a Looker Studio data source, which defines a connection to an underlying data set and its field schema. Data sources can be reusable (shared across reports) or embedded within a specific report.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the data source, serving as its unique identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the data source.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the data source owner.\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"email\",\n      \"description\": \"The email address of the user who created the data source.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the data source was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the data source was last modified.\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the data source has been moved to the trash.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of connector used by this data source.\",\n      \"enum\": [\n        \"bigQuery\",\n        \"cloudSpanner\",\n        \"communityConnector\",\n        \"googleAnalytics\",\n        \"googleCloudStorage\",\n        \"googleSheets\",\n        \"looker\",\n        \"searchConsole\"\n      ]\n    },\n\
  \    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"The field definitions that make up the data source schema.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Field\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"title\"\n  ],\n  \"$defs\": {\n    \"Field\": {\n      \"type\": \"object\",\n      \"description\": \"Defines a single field in the data source schema.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the field.\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"The display name for the field.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A text description of the field's contents.\"\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the field values.\",\n          \"enum\": [\n\
  \            \"STRING\",\n            \"NUMBER\",\n            \"BOOLEAN\"\n          ]\n        },\n        \"conceptType\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the field is a dimension (category) or metric (measurement).\",\n          \"enum\": [\n            \"DIMENSION\",\n            \"METRIC\"\n          ]\n        },\n        \"semanticType\": {\n          \"type\": \"string\",\n          \"description\": \"The semantic type describing the meaning of the field values.\",\n          \"enum\": [\n            \"TEXT\",\n            \"NUMBER\",\n            \"BOOLEAN\",\n            \"PERCENT\",\n            \"CURRENCY_USD\",\n            \"CURRENCY_EUR\",\n            \"CURRENCY_GBP\",\n            \"CURRENCY_JPY\",\n            \"YEAR\",\n            \"YEAR_QUARTER\",\n            \"YEAR_MONTH\",\n            \"YEAR_MONTH_DAY\",\n            \"YEAR_MONTH_DAY_HOUR\",\n            \"YEAR_MONTH_DAY_SECOND\",\n            \"QUARTER\",\n           \
  \ \"MONTH\",\n            \"WEEK\",\n            \"DAY_OF_WEEK\",\n            \"HOUR\",\n            \"MINUTE\",\n            \"DURATION\",\n            \"COUNTRY\",\n            \"COUNTRY_CODE\",\n            \"CONTINENT\",\n            \"CONTINENT_CODE\",\n            \"SUB_CONTINENT\",\n            \"SUB_CONTINENT_CODE\",\n            \"REGION\",\n            \"REGION_CODE\",\n            \"CITY\",\n            \"CITY_CODE\",\n            \"METRO\",\n            \"METRO_CODE\",\n            \"LATITUDE_LONGITUDE\",\n            \"URL\"\n          ]\n        },\n        \"defaultAggregationType\": {\n          \"type\": \"string\",\n          \"description\": \"The default aggregation type for metric fields.\",\n          \"enum\": [\n            \"AVG\",\n            \"COUNT\",\n            \"COUNT_DISTINCT\",\n            \"MAX\",\n            \"MIN\",\n            \"SUM\",\n            \"AUTO\",\n            \"NONE\"\n          ]\n        },\n        \"group\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"An optional group name for organizing related fields.\"\n        },\n        \"formula\": {\n          \"type\": \"string\",\n          \"description\": \"An optional calculated field formula.\"\n        },\n        \"isDefault\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this field is included by default in new charts.\"\n        },\n        \"isHidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the field is hidden from the user interface.\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"dataType\",\n        \"conceptType\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/json-schema/looker-studio-data-source-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
title: Looker Studio Data Source
---
