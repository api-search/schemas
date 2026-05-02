---
description: Represents a Looker Studio report, which is a collection of pages containing charts, tables, and other visualizations connected to one or more data sources.
layout: schema
name: Looker Studio Report
properties_list:
- description: The resource name of the report, serving as its unique identifier.
  name: name
  type: string
- description: The display title of the report.
  name: title
  type: string
- description: A text description of the report's purpose and contents.
  name: description
  type: string
- description: The email address of the report owner.
  name: owner
  type: string
- description: The email address of the user who originally created the report.
  name: creator
  type: string
- description: The timestamp when the report was created.
  name: createTime
  type: string
- description: The timestamp when the report was last modified.
  name: updateTime
  type: string
- description: Whether the report has been moved to the trash.
  name: trashed
  type: boolean
- description: The pages contained within this report.
  name: pages
  type: array
- description: The data sources connected to this report.
  name: dataSources
  type: array
provider_name: Looker Studio
provider_slug: looker-studio
schema_file: json-schema/looker-studio-report-schema.json
slug: looker-studio-report
source_filename: looker-studio-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/looker-studio/json-schema/looker-studio-report-schema.json\",\n  \"title\": \"Looker Studio Report\",\n  \"description\": \"Represents a Looker Studio report, which is a collection of pages containing charts, tables, and other visualizations connected to one or more data sources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the report, serving as its unique identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the report.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A text description of the report's purpose and contents.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the report\
  \ owner.\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user who originally created the report.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the report was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the report was last modified.\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the report has been moved to the trash.\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"The pages contained within this report.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Page\"\n      }\n    },\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"description\": \"The data sources connected to this report.\",\n      \"items\": {\n\
  \        \"$ref\": \"#/$defs/DataSourceReference\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"title\"\n  ],\n  \"$defs\": {\n    \"Page\": {\n      \"type\": \"object\",\n      \"description\": \"A single page within a Looker Studio report.\",\n      \"properties\": {\n        \"pageId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for this page within the report.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the page.\"\n        },\n        \"hidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this page is hidden from viewers.\"\n        }\n      },\n      \"required\": [\n        \"pageId\"\n      ]\n    },\n    \"DataSourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a data source used by the report.\",\n      \"properties\": {\n        \"alias\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The alias identifier for the data source within the report (e.g., ds0, ds1).\"\n        },\n        \"dataSourceName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the data source.\"\n        },\n        \"connectorType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of connector used by this data source.\",\n          \"enum\": [\n            \"bigQuery\",\n            \"cloudSpanner\",\n            \"communityConnector\",\n            \"googleAnalytics\",\n            \"googleCloudStorage\",\n            \"googleSheets\",\n            \"looker\",\n            \"searchConsole\"\n          ]\n        }\n      },\n      \"required\": [\n        \"alias\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/json-schema/looker-studio-report-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
title: Looker Studio Report
---
