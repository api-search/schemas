---
description: CreateQueueRequest schema from Amazon MediaConvert API
layout: schema
name: CreateQueueRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PricingPlan
  type: object
- description: ''
  name: ReservationPlanSettings
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-create-queue-request-schema.json
slug: mediaconvert-api-create-queue-request
source_filename: mediaconvert-api-create-queue-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-queue-request-schema.json\",\n  \"title\": \"CreateQueueRequest\",\n  \"description\": \"CreateQueueRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"Optional. A description of the queue that you are creating.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the queue that you are creating.\"\
  \n        }\n      ]\n    },\n    \"PricingPlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingPlan\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pricingPlan\"\n          },\n          \"description\": \"Specifies whether the pricing plan for the queue is on-demand or reserved. For on-demand, you pay per minute, billed in increments of .01 minute. For reserved, you pay for the transcoding capacity of the entire queue, regardless of how much or how little you use it. Reserved pricing requires a 12-month commitment. When you use the API to create a queue, the default is on-demand.\"\n        }\n      ]\n    },\n    \"ReservationPlanSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationPlanSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservationPlanSettings\"\n          },\n          \"description\": \"Details about the pricing plan for your reserved\
  \ queue. Required for reserved queues and not applicable to on-demand queues.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueueStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Initial state of the queue. If you create a paused queue, then jobs in that queue won't begin.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags that you want to add to the resource. You can tag resources with a key-value pair or with only a key.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-create-queue-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateQueueRequest
---
