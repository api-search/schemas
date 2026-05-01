---
description: Represents a Looker Studio report, which is a customizable dashboard or report asset that connects to data sources and presents data through visualizations. Reports are a subtype of Asset with assetType REPORT.
layout: schema
name: Looker Studio Report
properties_list:
- description: The asset type, always REPORT for report assets.
  name: assetType
  type: string
- description: The unique name (ID) of the report. Used as the asset identifier in API calls and Linking API URLs.
  name: name
  type: string
- description: The display title of the report.
  name: title
  type: string
- description: Description of the report providing context about its purpose and contents.
  name: description
  type: string
- description: The email address of the report owner.
  name: owner
  type: string
- description: The email address of the user who originally created the report.
  name: creator
  type: string
- description: Timestamp when the report was created, in RFC 3339 format.
  name: createTime
  type: string
- description: Timestamp when the report was last modified, in RFC 3339 format.
  name: updateTime
  type: string
- description: Timestamp when the report was last modified by the authenticated user, in RFC 3339 format.
  name: updateByMeTime
  type: string
- description: Timestamp when the report was last viewed by the authenticated user, in RFC 3339 format.
  name: lastViewByMeTime
  type: string
- description: Indicates whether the report is currently in the trash.
  name: trashed
  type: boolean
provider_name: Google Data Studio
provider_slug: google-data-studio
schema_file: json-schema/google-data-studio-report-schema.json
slug: google-data-studio-report
source_filename: google-data-studio-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"google-data-studio-report-schema.json\",\n  \"title\": \"Looker Studio Report\",\n  \"description\": \"Represents a Looker Studio report, which is a customizable dashboard or report asset that connects to data sources and presents data through visualizations. Reports are a subtype of Asset with assetType REPORT.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"assetType\",\n    \"name\",\n    \"title\",\n    \"owner\",\n    \"creator\",\n    \"createTime\",\n    \"updateTime\"\n  ],\n  \"properties\": {\n    \"assetType\": {\n      \"type\": \"string\",\n      \"description\": \"The asset type, always REPORT for report assets.\",\n      \"const\": \"REPORT\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name (ID) of the report. Used as the asset identifier in API calls and Linking API URLs.\"\n    },\n    \"title\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The display title of the report.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the report providing context about its purpose and contents.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the report owner.\",\n      \"format\": \"email\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user who originally created the report.\",\n      \"format\": \"email\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the report was created, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the report was last modified, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"updateByMeTime\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Timestamp when the report was last modified by the authenticated user, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"lastViewByMeTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the report was last viewed by the authenticated user, in RFC 3339 format.\",\n      \"format\": \"date-time\"\n    },\n    \"trashed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the report is currently in the trash.\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/json-schema/google-data-studio-report-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
title: Looker Studio Report
---
