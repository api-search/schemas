---
description: Specifies the conditions for the first activity in a journey. This activity and its conditions determine which users are participants in a journey.
layout: schema
name: StartCondition
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: EventStartCondition
  type: object
- description: ''
  name: SegmentStartCondition
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-start-condition-schema.json
slug: amazon-pinpoint-start-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-start-condition-schema.json\",\n  \"title\": \"StartCondition\",\n  \"description\": \"Specifies the conditions for the first activity in a journey. This activity and its conditions determine which users are participants in a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the condition.\"\n        }\n      ]\n    },\n    \"EventStartCondition\": {\n      \"$ref\": \"#/components/schemas/EventStartCondition\"\n    },\n    \"SegmentStartCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentCondition\"\n        },\n        {\n          \"description\"\
  : \"The segment that's associated with the first activity in the journey. This segment determines which users are participants in the journey.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-start-condition-schema.json
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
title: StartCondition
---
