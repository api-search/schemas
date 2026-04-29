---
description: UpdateQueueRequest schema from Amazon MediaConvert API
layout: schema
name: UpdateQueueRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: ReservationPlanSettings
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-update-queue-request-schema.json
slug: mediaconvert-api-update-queue-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-queue-request-schema.json\",\n  \"title\": \"UpdateQueueRequest\",\n  \"description\": \"UpdateQueueRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The new description for the queue, if you are changing it.\"\n        }\n      ]\n    },\n    \"ReservationPlanSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationPlanSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservationPlanSettings\"\n          },\n          \"description\"\
  : \"The new details of your pricing plan for your reserved queue. When you set up a new pricing plan to replace an expired one, you enter into another 12-month commitment. When you add capacity to your queue by increasing the number of RTS, you extend the term of your commitment to 12 months from when you add capacity. After you make these commitments, you can't cancel them.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueueStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Pause or activate a queue by changing its status between ACTIVE and PAUSED. If you pause a queue, jobs in that queue won't begin. Jobs that are running when you pause the queue continue to run until they finish or result in an error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-queue-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateQueueRequest
---
