---
description: Provides information about the status, configuration, and other settings for a journey.
layout: schema
name: JourneyResponse
properties_list:
- description: ''
  name: Activities
  type: object
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Id
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
  name: tags
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
schema_file: json-schema/amazon-pinpoint-journey-response-schema.json
slug: amazon-pinpoint-journey-response
source_filename: amazon-pinpoint-journey-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-response-schema.json\",\n  \"title\": \"JourneyResponse\",\n  \"description\": \"Provides information about the status, configuration, and other settings for a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfActivity\"\n        },\n        {\n          \"description\": \"A map that contains a set of Activity objects, one object for each activity in the journey. For each Activity object, the key is the unique identifier (string) for an activity and the value is the settings for the activity.\"\n        }\n      ]\n    },\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"The unique identifier for the application that the journey applies to.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the journey was created.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the journey.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the journey was last modified.\"\n        }\n      ]\n    },\n    \"Limits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneyLimits\"\n        },\n        {\n          \"description\"\
  : \"The messaging and entry limits for the journey.\"\n        }\n      ]\n    },\n    \"LocalTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the journey's scheduled start and end times use each participant's local time. If this value is true, the schedule uses each participant's local time.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the journey.\"\n        }\n      ]\n    },\n    \"QuietTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuietTime\"\n        },\n        {\n          \"description\": \"<p>The quiet time settings for the journey. Quiet time is a specific time range when a journey doesn't send messages to participants, if all the following conditions are met:</p> <ul><li><p>The\
  \ EndpointDemographic.Timezone property of the endpoint for the participant is set to a valid value.</p></li> <li><p>The current time in the participant's time zone is later than or equal to the time specified by the QuietTime.Start property for the journey.</p></li> <li><p>The current time in the participant's time zone is earlier than or equal to the time specified by the QuietTime.End property for the journey.</p></li></ul> <p>If any of the preceding conditions isn't met, the participant will receive messages from the journey, even if quiet time is enabled.</p>\"\n        }\n      ]\n    },\n    \"RefreshFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The frequency with which Amazon Pinpoint evaluates segment and event data for the journey, as a duration in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/JourneySchedule\"\n        },\n        {\n          \"description\": \"The schedule settings for the journey.\"\n        }\n      ]\n    },\n    \"StartActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the first activity in the journey.\"\n        }\n      ]\n    },\n    \"StartCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartCondition\"\n        },\n        {\n          \"description\": \"The segment that defines which users are participants in the journey.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"<p>The current status of the journey. Possible values are:</p> <ul><li><p>DRAFT - The journey is being developed and hasn't been published yet.</p></li> <li><p>ACTIVE\
  \ - The journey has been developed and published. Depending on the journey's schedule, the journey may currently be running or scheduled to start running at a later time. If a journey's status is ACTIVE, you can't add, change, or remove activities from it.</p></li> <li><p>COMPLETED - The journey has been published and has finished running. All participants have entered the journey and no participants are waiting to complete the journey or any activities in the journey.</p></li> <li><p>CANCELLED - The journey has been stopped. If a journey's status is CANCELLED, you can't add, change, or remove activities or segment settings from the journey.</p></li> <li><p>CLOSED - The journey has been published and has started running. It may have also passed its scheduled end time, or passed its scheduled start time and a refresh frequency hasn't been specified for it. If a journey's status is CLOSED, you can't add participants to it, and no existing participants can enter the journey for the first\
  \ time. However, any existing participants who are currently waiting to start an activity may continue the journey.</p></li></ul>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"This object is not used or supported.\"\n        }\n      ]\n    },\n    \"WaitForQuietTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether endpoints in quiet hours should enter a wait till the end of their quiet hours.\"\n        }\n      ]\n    },\n    \"RefreshOnSegmentUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether a journey should be refreshed on segment update.\"\n        }\n      ]\n    },\n    \"JourneyChannelSettings\": {\n     \
  \ \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JourneyChannelSettings\"\n        },\n        {\n          \"description\": \"The channel-specific configurations for the journey.\"\n        }\n      ]\n    },\n    \"SendingSchedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Indicates if journey have Advance Quiet Time (OpenHours and ClosedDays). This flag should be set to true in order to allow (OpenHours and ClosedDays)\"\n        }\n      ]\n    },\n    \"OpenHours\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenHours\"\n        },\n        {\n          \"description\": \"The time when journey allow to send messages. QuietTime should be configured first and SendingSchedule should be set to true.\"\n        }\n      ]\n    },\n    \"ClosedDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClosedDays\"\
  \n        },\n        {\n          \"description\": \"The time when journey will stop sending messages. QuietTime should be configured first and SendingSchedule should be set to true.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Id\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-response-schema.json
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
title: JourneyResponse
---
