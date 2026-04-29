---
description: A date-time value with a time zone designation.
layout: schema
name: DateTimeTimeZone
properties_list:
- description: A single point of time in a combined date and time representation (e.g. 2017-08-29T04:00:00.0000000).
  name: dateTime
  type: string
- description: Represents a time zone, for example, Pacific Standard Time.
  name: timeZone
  type: string
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-date-time-time-zone-schema.json
slug: microsoft-graph-mail-date-time-time-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DateTimeTimeZone\",\n  \"type\": \"object\",\n  \"description\": \"A date-time value with a time zone designation.\",\n  \"properties\": {\n    \"dateTime\": {\n      \"type\": \"string\",\n      \"description\": \"A single point of time in a combined date and time representation (e.g. 2017-08-29T04:00:00.0000000).\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Represents a time zone, for example, Pacific Standard Time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-date-time-time-zone-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: DateTimeTimeZone
---
