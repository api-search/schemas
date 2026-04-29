---
description: Provides information about an activity that was performed by a campaign.
layout: schema
name: ActivityResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: CampaignId
  type: object
- description: ''
  name: End
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Result
  type: object
- description: ''
  name: ScheduledStart
  type: object
- description: ''
  name: Start
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: SuccessfulEndpointCount
  type: object
- description: ''
  name: TimezonesCompletedCount
  type: object
- description: ''
  name: TimezonesTotalCount
  type: object
- description: ''
  name: TotalEndpointCount
  type: object
- description: ''
  name: TreatmentId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-activity-response-schema.json
slug: amazon-pinpoint-activity-response
source_filename: amazon-pinpoint-activity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-activity-response-schema.json\",\n  \"title\": \"ActivityResponse\",\n  \"description\": \"Provides information about an activity that was performed by a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the campaign applies to.\"\n        }\n      ]\n    },\n    \"CampaignId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the campaign that the activity applies to.\"\n        }\n      ]\n    },\n    \"End\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The actual time, in ISO 8601 format, when the activity was marked CANCELLED or COMPLETED.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the activity.\"\n        }\n      ]\n    },\n    \"Result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Specifies whether the activity succeeded. Possible values are SUCCESS and FAIL.\"\n        }\n      ]\n    },\n    \"ScheduledStart\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The scheduled start time, in ISO 8601 format, for the activity.\"\n        }\n      ]\n    },\n    \"Start\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The actual start time, in ISO 8601 format, of the activity.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The current status of the activity. Possible values are: PENDING, INITIALIZING, RUNNING, PAUSED, CANCELLED, and COMPLETED.\"\n        }\n      ]\n    },\n    \"SuccessfulEndpointCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total number of endpoints that the campaign successfully delivered messages to.\"\n        }\n      ]\n    },\n    \"TimezonesCompletedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The\
  \ total number of time zones that were completed.\"\n        }\n      ]\n    },\n    \"TimezonesTotalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total number of unique time zones that are in the segment for the campaign.\"\n        }\n      ]\n    },\n    \"TotalEndpointCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total number of endpoints that the campaign attempted to deliver messages to.\"\n        }\n      ]\n    },\n    \"TreatmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the campaign treatment that the activity applies to. A treatment is a variation of a campaign that's used for A/B testing of a campaign.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"CampaignId\",\n    \"Id\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-activity-response-schema.json
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
title: ActivityResponse
---
