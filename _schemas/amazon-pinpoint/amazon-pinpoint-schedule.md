---
description: Specifies the schedule settings for a campaign.
layout: schema
name: Schedule
properties_list:
- description: ''
  name: EndTime
  type: object
- description: ''
  name: EventFilter
  type: object
- description: ''
  name: Frequency
  type: object
- description: ''
  name: IsLocalTime
  type: object
- description: ''
  name: QuietTime
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Timezone
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-schedule-schema.json
slug: amazon-pinpoint-schedule
source_filename: amazon-pinpoint-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-schedule-schema.json\",\n  \"title\": \"Schedule\",\n  \"description\": \"Specifies the schedule settings for a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The scheduled time, in ISO 8601 format, when the campaign ended or will end.\"\n        }\n      ]\n    },\n    \"EventFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignEventFilter\"\n        },\n        {\n          \"description\": \"The type of event that causes the campaign to be sent, if the value of the Frequency property is EVENT.\"\n        }\n      ]\n    },\n    \"Frequency\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"Specifies how often the campaign is sent or whether the campaign is sent in response to a specific event.\"\n        }\n      ]\n    },\n    \"IsLocalTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the start and end times for the campaign schedule use each recipient's local time. To base the schedule on each recipient's local time, set this value to true.\"\n        }\n      ]\n    },\n    \"QuietTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuietTime\"\n        },\n        {\n          \"description\": \"<p>The default quiet time for the campaign. Quiet time is a specific time range when a campaign doesn't send messages to endpoints, if all the following conditions are met:</p> <ul><li><p>The EndpointDemographic.Timezone\
  \ property of the endpoint is set to a valid value.</p></li> <li><p>The current time in the endpoint's time zone is later than or equal to the time specified by the QuietTime.Start property for the campaign.</p></li> <li><p>The current time in the endpoint's time zone is earlier than or equal to the time specified by the QuietTime.End property for the campaign.</p></li></ul> <p>If any of the preceding conditions isn't met, the endpoint will receive messages from the campaign, even if quiet time is enabled.</p>\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The scheduled time when the campaign began or will begin. Valid values are: IMMEDIATE, to start the campaign immediately; or, a specific time in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The starting UTC offset for the campaign schedule, if the value of the IsLocalTime property is true. Valid values are: UTC, UTC+01, UTC+02, UTC+03, UTC+03:30, UTC+04, UTC+04:30, UTC+05,\\n                  UTC+05:30, UTC+05:45, UTC+06, UTC+06:30, UTC+07, UTC+08, UTC+09, UTC+09:30,\\n                  UTC+10, UTC+10:30, UTC+11, UTC+12, UTC+13, UTC-02, UTC-03, UTC-04, UTC-05, UTC-06,\\n                  UTC-07, UTC-08, UTC-09, UTC-10, and UTC-11.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StartTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-schedule-schema.json
tags:
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
title: Schedule
---
