---
description: You can use queues to manage the resources that are available to your AWS account for running multiple transcoding jobs at the same time. If you don't specify a queue, the service sends all jobs through the default queue. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/working-with-queues.html.
layout: schema
name: Queue
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LastUpdated
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PricingPlan
  type: object
- description: ''
  name: ProgressingJobsCount
  type: object
- description: ''
  name: ReservationPlan
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SubmittedJobsCount
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-queue-schema.json
slug: mediaconvert-api-queue
source_filename: mediaconvert-api-queue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-schema.json\",\n  \"title\": \"Queue\",\n  \"description\": \"You can use queues to manage the resources that are available to your AWS account for running multiple transcoding jobs at the same time. If you don't specify a queue, the service sends all jobs through the default queue. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/working-with-queues.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"An identifier for this resource that is unique within all of AWS.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The timestamp in epoch seconds for when you created the queue.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"An optional description that you create for each queue.\"\n        }\n      ]\n    },\n    \"LastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lastUpdated\"\n          },\n          \"description\": \"The timestamp in epoch seconds for when you most recently updated the queue.\"\n        }\n      ]\n    },\n    \"Name\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"A name that you create for each queue. Each name must be unique within your account.\"\n        }\n      ]\n    },\n    \"PricingPlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PricingPlan\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pricingPlan\"\n          },\n          \"description\": \"Specifies whether the pricing plan for the queue is on-demand or reserved. For on-demand, you pay per minute, billed in increments of .01 minute. For reserved, you pay for the transcoding capacity of the entire queue, regardless of how much or how little you use it. Reserved pricing requires a 12-month commitment.\"\n        }\n      ]\n    },\n    \"ProgressingJobsCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"progressingJobsCount\"\n          },\n          \"description\": \"The estimated number of jobs with a PROGRESSING status.\"\n        }\n      ]\n    },\n    \"ReservationPlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationPlan\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservationPlan\"\n          },\n          \"description\": \"Details about the pricing plan for your reserved queue. Required for reserved queues and not applicable to on-demand queues.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueueStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Queues can be ACTIVE or PAUSED. If you pause a queue, the service won't begin processing jobs in that queue. Jobs that are running when you\
  \ pause the queue continue to run until they finish or result in an error.\"\n        }\n      ]\n    },\n    \"SubmittedJobsCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"submittedJobsCount\"\n          },\n          \"description\": \"The estimated number of jobs with a SUBMITTED status.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"Specifies whether this on-demand queue is system or custom. System queues are built in. You can't modify or delete system queues. You can create and modify custom queues.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Queue
---
