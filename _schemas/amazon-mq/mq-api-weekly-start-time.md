---
description: The scheduled time period relative to UTC during which Amazon MQ begins to apply pending updates or patches to the broker.
layout: schema
name: WeeklyStartTime
properties_list:
- description: ''
  name: DayOfWeek
  type: object
- description: ''
  name: TimeOfDay
  type: object
- description: ''
  name: TimeZone
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-weekly-start-time-schema.json
slug: mq-api-weekly-start-time
source_filename: mq-api-weekly-start-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-weekly-start-time-schema.json\",\n  \"title\": \"WeeklyStartTime\",\n  \"description\": \"The scheduled time period relative to UTC during which Amazon MQ begins to apply pending updates or patches to the broker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DayOfWeek\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfWeek\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dayOfWeek\"\n          },\n          \"description\": \"Required. The day of the week.\"\n        }\n      ]\n    },\n    \"TimeOfDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timeOfDay\"\n          },\n          \"description\": \"Required. The time,\
  \ in 24-hour format.\"\n        }\n      ]\n    },\n    \"TimeZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timeZone\"\n          },\n          \"description\": \"The time zone, UTC by default, in either the Country/City format, or the UTC offset format.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TimeOfDay\",\n    \"DayOfWeek\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-weekly-start-time-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: WeeklyStartTime
---
