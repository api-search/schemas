---
description: A public holiday calendar in absentify.
layout: schema
name: PublicHolidayCalendar
properties_list:
- description: Unique identifier of the calendar.
  name: id
  type: string
- description: Name of the public holiday calendar.
  name: name
  type: string
- description: Country code for the public holidays.
  name: country
  type: string
- description: Timestamp when the calendar was created.
  name: createdAt
  type: string
- description: Timestamp when the calendar was last updated.
  name: updatedAt
  type: string
provider_name: Absentify
provider_slug: absentify
schema_file: json-schema/absentify-public-holiday-calendar-schema.json
slug: absentify-public-holiday-calendar
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absentify/main/json-schema/absentify-public-holiday-calendar-schema.json\",\n  \"title\": \"PublicHolidayCalendar\",\n  \"description\": \"A public holiday calendar in absentify.\",\n  \"type\": \"object\",\n  \"x-schema-source\": \"openapi-spec\",\n  \"x-provider\": \"absentify\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the calendar.\",\n      \"example\": \"500888\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the public holiday calendar.\",\n      \"example\": \"United States Federal Holidays\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code for the public holidays.\",\n      \"example\": \"US\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp when the calendar was created.\",\n      \"example\": \"2025-01-01T00:00:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the calendar was last updated.\",\n      \"example\": \"2025-06-01T09:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absentify/refs/heads/main/json-schema/absentify-public-holiday-calendar-schema.json
tags:
- Absence Management
- HR
- Leave Management
- Microsoft Teams
- Human Resources
title: PublicHolidayCalendar
---
