---
description: Schedule configuration for automated report generation and delivery.
layout: schema
name: ReportSchedule
properties_list:
- description: Whether the schedule is active.
  name: active
  type: boolean
- description: The interval at which the report is run. Acceptable values are DAILY, WEEKLY, MONTHLY, or QUARTERLY.
  name: repeats
  type: string
- description: Defines every how many days, weeks, or months the report should be run.
  name: every
  type: integer
- description: Start date of the scheduled reports.
  name: startDate
  type: string
- description: The expiration date when the scheduled report stops running.
  name: expirationDate
  type: string
- description: Enum to define for MONTHLY and QUARTERLY schedules whether reports should be repeated on the same day of the month or the same day of the week.
  name: runsOnDayOfMonth
  type: string
- description: The timezone for the report schedule.
  name: timezone
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-report-schedule-schema.json
slug: google-campaign-manager-report-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportSchedule\",\n  \"type\": \"object\",\n  \"description\": \"Schedule configuration for automated report generation and delivery.\",\n  \"properties\": {\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the schedule is active.\"\n    },\n    \"repeats\": {\n      \"type\": \"string\",\n      \"description\": \"The interval at which the report is run. Acceptable values are DAILY, WEEKLY, MONTHLY, or QUARTERLY.\"\n    },\n    \"every\": {\n      \"type\": \"integer\",\n      \"description\": \"Defines every how many days, weeks, or months the report should be run.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Start date of the scheduled reports.\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The expiration date when the scheduled report stops running.\"\n    },\n    \"runsOnDayOfMonth\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Enum to define for MONTHLY and QUARTERLY schedules whether reports should be repeated on the same day of the month or the same day of the week.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The timezone for the report schedule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-report-schedule-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ReportSchedule
---
