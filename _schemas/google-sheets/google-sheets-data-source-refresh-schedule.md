---
description: Schedule for refreshing a data source.
layout: schema
name: DataSourceRefreshSchedule
properties_list:
- description: True if the refresh schedule is enabled.
  name: enabled
  type: boolean
- description: The scope of the refresh.
  name: refreshScope
  type: string
- description: Output only. The time interval of the next run.
  name: nextRun
  type: object
- description: Daily refresh schedule.
  name: dailySchedule
  type: object
- description: Weekly refresh schedule.
  name: weeklySchedule
  type: object
- description: Monthly refresh schedule.
  name: monthlySchedule
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-refresh-schedule-schema.json
slug: google-sheets-data-source-refresh-schedule
source_filename: google-sheets-data-source-refresh-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceRefreshSchedule\",\n  \"type\": \"object\",\n  \"description\": \"Schedule for refreshing a data source.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the refresh schedule is enabled.\"\n    },\n    \"refreshScope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope of the refresh.\"\n    },\n    \"nextRun\": {\n      \"type\": \"object\",\n      \"description\": \"Output only. The time interval of the next run.\"\n    },\n    \"dailySchedule\": {\n      \"type\": \"object\",\n      \"description\": \"Daily refresh schedule.\"\n    },\n    \"weeklySchedule\": {\n      \"type\": \"object\",\n      \"description\": \"Weekly refresh schedule.\"\n    },\n    \"monthlySchedule\": {\n      \"type\": \"object\",\n      \"description\": \"Monthly refresh schedule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-refresh-schedule-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSourceRefreshSchedule
---
