---
description: Specifies the schedule settings for a journey.
layout: schema
name: JourneySchedule
properties_list:
- description: ''
  name: EndTime
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Timezone
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-schedule-schema.json
slug: amazon-pinpoint-journey-schedule
source_filename: amazon-pinpoint-journey-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-schedule-schema.json\",\n  \"title\": \"JourneySchedule\",\n  \"description\": \"Specifies the schedule settings for a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The scheduled time, in ISO 8601 format, when the journey ended or will end.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The scheduled time, in ISO 8601 format, when the journey began or will begin.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The starting UTC offset for the journey schedule, if the value of the journey's LocalTime property is true. Valid values are: UTC,\\n                  UTC+01, UTC+02, UTC+03, UTC+03:30, UTC+04, UTC+04:30, UTC+05, UTC+05:30,\\n                  UTC+05:45, UTC+06, UTC+06:30, UTC+07, UTC+08, UTC+08:45, UTC+09, UTC+09:30,\\n                  UTC+10, UTC+10:30, UTC+11, UTC+12, UTC+12:45, UTC+13, UTC+13:45, UTC-02,\\n                  UTC-02:30, UTC-03, UTC-03:30, UTC-04, UTC-05, UTC-06, UTC-07, UTC-08, UTC-09,\\n                  UTC-09:30, UTC-10, and UTC-11.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-schedule-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: JourneySchedule
---
