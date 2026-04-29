---
description: Day part targeting configuration.
layout: schema
name: DayPartTargeting
properties_list:
- description: Whether targeting is based on user's local time.
  name: userLocalTime
  type: boolean
- description: Hours of the day to target (0-23).
  name: hoursOfDay
  type: array
- description: Days of the week to target.
  name: daysOfWeek
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-day-part-targeting-schema.json
slug: google-campaign-manager-day-part-targeting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DayPartTargeting\",\n  \"type\": \"object\",\n  \"description\": \"Day part targeting configuration.\",\n  \"properties\": {\n    \"userLocalTime\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether targeting is based on user's local time.\"\n    },\n    \"hoursOfDay\": {\n      \"type\": \"array\",\n      \"description\": \"Hours of the day to target (0-23).\"\n    },\n    \"daysOfWeek\": {\n      \"type\": \"array\",\n      \"description\": \"Days of the week to target.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-day-part-targeting-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: DayPartTargeting
---
