---
description: Specifies the configuration and other settings for a journey.
layout: schema
name: WriteJourneyRequest
properties_list:
- description: ''
  name: Activities
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Limits
  type: object
- description: ''
  name: LocalTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: QuietTime
  type: object
- description: ''
  name: RefreshFrequency
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: StartActivity
  type: object
- description: ''
  name: StartCondition
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: WaitForQuietTime
  type: object
- description: ''
  name: RefreshOnSegmentUpdate
  type: object
- description: ''
  name: JourneyChannelSettings
  type: object
- description: ''
  name: SendingSchedule
  type: object
- description: ''
  name: OpenHours
  type: object
- description: ''
  name: ClosedDays
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-write-journey-request-schema.json
slug: amazon-pinpoint-write-journey-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-write-journey-request-schema.json\",\n  \"title\": \"WriteJourneyRequest\",\n  \"description\": \"Specifies the configuration and other settings for a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfActivity\"\n        },\n        {\n          \"description\": \"A map that contains a set of Activity objects, one object for each activity in the journey. For each Activity object, the key is the unique identifier (string) for an activity and the value is the settings for the activity. An activity identifier can contain a maximum of 100 characters. The characters must be alphanumeric characters.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the journey was created.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the journey was last modified.\"\n        }\n      ]\n    },\n    \"Limits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneyLimits\"\n        },\n        {\n          \"description\": \"The messaging and entry limits for the journey.\"\n        }\n      ]\n    },\n    \"LocalTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the journey's scheduled start and end times use each participant's local time. To base the schedule on each participant's\
  \ local time, set this value to true.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the journey. A journey name can contain a maximum of 150 characters. The characters can be alphanumeric characters or symbols, such as underscores (_) or hyphens (-). A journey name can't contain any spaces.\"\n        }\n      ]\n    },\n    \"QuietTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuietTime\"\n        },\n        {\n          \"description\": \"<p>The quiet time settings for the journey. Quiet time is a specific time range when a journey doesn't send messages to participants, if all the following conditions are met:</p> <ul><li><p>The EndpointDemographic.Timezone property of the endpoint for the participant is set to a valid value.</p></li> <li><p>The current time in the participant's time zone is later\
  \ than or equal to the time specified by the QuietTime.Start property for the journey.</p></li> <li><p>The current time in the participant's time zone is earlier than or equal to the time specified by the QuietTime.End property for the journey.</p></li></ul> <p>If any of the preceding conditions isn't met, the participant will receive messages from the journey, even if quiet time is enabled.</p>\"\n        }\n      ]\n    },\n    \"RefreshFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The frequency with which Amazon Pinpoint evaluates segment and event data for the journey, as a duration in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneySchedule\"\n        },\n        {\n          \"description\": \"The schedule settings for the journey.\"\n        }\n      ]\n    },\n    \"StartActivity\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the first activity in the journey. The identifier for this activity can contain a maximum of 128 characters. The characters must be alphanumeric characters.\"\n        }\n      ]\n    },\n    \"StartCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartCondition\"\n        },\n        {\n          \"description\": \"The segment that defines which users are participants in the journey.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"<p>The status of the journey. Valid values are:</p> <ul><li><p>DRAFT - Saves the journey and doesn't publish it.</p></li> <li><p>ACTIVE - Saves and publishes the journey. Depending on the journey's schedule, the journey\
  \ starts running immediately or at the scheduled start time. If a journey's status is ACTIVE, you can't add, change, or remove activities from it.</p></li></ul> <p>PAUSED, CANCELLED, COMPLETED, and CLOSED states are not supported in requests to create or update a journey. To cancel, pause, or resume a journey, use the <link  linkend=\\\"apps-application-id-journeys-journey-id-state\\\">Journey State</link> resource.</p>\"\n        }\n      ]\n    },\n    \"WaitForQuietTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether endpoints in quiet hours should enter a wait till the end of their quiet hours.\"\n        }\n      ]\n    },\n    \"RefreshOnSegmentUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether a journey should be refreshed on segment update.\"\n   \
  \     }\n      ]\n    },\n    \"JourneyChannelSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneyChannelSettings\"\n        },\n        {\n          \"description\": \"The channel-specific configurations for the journey.\"\n        }\n      ]\n    },\n    \"SendingSchedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Indicates if journey have Advance Quiet Time (OpenHours and ClosedDays). This flag should be set to true in order to allow (OpenHours and ClosedDays)\"\n        }\n      ]\n    },\n    \"OpenHours\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenHours\"\n        },\n        {\n          \"description\": \"The time when journey allow to send messages. QuietTime should be configured first and SendingSchedule should be set to true.\"\n        }\n      ]\n    },\n    \"ClosedDays\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ClosedDays\"\n        },\n        {\n          \"description\": \"The time when journey will stop sending messages. QuietTime should be configured first and SendingSchedule should be set to true.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-write-journey-request-schema.json
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
title: WriteJourneyRequest
---
