---
description: Recurrence settings for recurring meetings.
layout: schema
name: Recurrence
properties_list:
- description: Recurrence type. 1 - Daily, 2 - Weekly, 3 - Monthly.
  name: type
  type: integer
- description: Interval at which the meeting recurs. For daily, max 90. For weekly, max 12. For monthly, max 3.
  name: repeat_interval
  type: integer
- description: Days of the week for weekly recurrence. 1-Sunday through 7-Saturday. Comma separated for multiple days.
  name: weekly_days
  type: string
- description: Day of the month for monthly recurrence (1-31).
  name: monthly_day
  type: integer
- description: Week of the month for monthly recurrence. -1 - Last week, 1 - First, 2 - Second, 3 - Third, 4 - Fourth.
  name: monthly_week
  type: integer
- description: Day of the week for monthly recurrence. 1-Sunday through 7-Saturday.
  name: monthly_week_day
  type: integer
- description: Number of times the meeting will recur before ending. Cannot be used with end_date_time. Maximum 365 for daily, 99 for weekly and monthly.
  name: end_times
  type: integer
- description: The end date-time for the recurrence. Cannot be used with end_times.
  name: end_date_time
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-recurrence-schema.json
slug: zoom-meeting-recurrence
source_filename: zoom-meeting-recurrence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Recurrence\",\n  \"type\": \"object\",\n  \"description\": \"Recurrence settings for recurring meetings.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"integer\",\n      \"description\": \"Recurrence type. 1 - Daily, 2 - Weekly, 3 - Monthly.\"\n    },\n    \"repeat_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval at which the meeting recurs. For daily, max 90. For weekly, max 12. For monthly, max 3.\"\n    },\n    \"weekly_days\": {\n      \"type\": \"string\",\n      \"description\": \"Days of the week for weekly recurrence. 1-Sunday through 7-Saturday. Comma separated for multiple days.\"\n    },\n    \"monthly_day\": {\n      \"type\": \"integer\",\n      \"description\": \"Day of the month for monthly recurrence (1-31).\"\n    },\n    \"monthly_week\": {\n      \"type\": \"integer\",\n      \"description\": \"Week of the month for monthly recurrence.\
  \ -1 - Last week, 1 - First, 2 - Second, 3 - Third, 4 - Fourth.\"\n    },\n    \"monthly_week_day\": {\n      \"type\": \"integer\",\n      \"description\": \"Day of the week for monthly recurrence. 1-Sunday through 7-Saturday.\"\n    },\n    \"end_times\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the meeting will recur before ending. Cannot be used with end_date_time. Maximum 365 for daily, 99 for weekly and monthly.\"\n    },\n    \"end_date_time\": {\n      \"type\": \"string\",\n      \"description\": \"The end date-time for the recurrence. Cannot be used with end_times.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-recurrence-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: Recurrence
---
