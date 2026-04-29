---
description: Describes the date, time, and time zone of a point in time.
layout: schema
name: DateTimeTimeZone
properties_list:
- description: A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).
  name: dateTime
  type: string
- description: The time zone for the time. For example, Pacific Standard Time. See https://learn.microsoft.com/en-us/graph/api/resources/datetimetimezone
  name: timeZone
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-date-time-time-zone-schema.json
slug: microsoft-graph-date-time-time-zone
source_filename: microsoft-graph-date-time-time-zone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DateTimeTimeZone\",\n  \"type\": \"object\",\n  \"description\": \"Describes the date, time, and time zone of a point in time.\",\n  \"properties\": {\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"description\": \"A single point of time in a combined date and time representation ({date}T{time}; for example, 2017-08-29T04:00:00.0000000).\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone for the time. For example, Pacific Standard Time. See https://learn.microsoft.com/en-us/graph/api/resources/datetimetimezone\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-date-time-time-zone-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: DateTimeTimeZone
---
