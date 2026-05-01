---
description: Details about the pricing plan for your reserved queue. Required for reserved queues and not applicable to on-demand queues.
layout: schema
name: ReservationPlan
properties_list:
- description: ''
  name: Commitment
  type: object
- description: ''
  name: ExpiresAt
  type: object
- description: ''
  name: PurchasedAt
  type: object
- description: ''
  name: RenewalType
  type: object
- description: ''
  name: ReservedSlots
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-reservation-plan-schema.json
slug: mediaconvert-api-reservation-plan
source_filename: mediaconvert-api-reservation-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-reservation-plan-schema.json\",\n  \"title\": \"ReservationPlan\",\n  \"description\": \"Details about the pricing plan for your reserved queue. Required for reserved queues and not applicable to on-demand queues.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Commitment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Commitment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"commitment\"\n          },\n          \"description\": \"The length of the term of your reserved queue pricing plan commitment.\"\n        }\n      ]\n    },\n    \"ExpiresAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"expiresAt\"\
  \n          },\n          \"description\": \"The timestamp in epoch seconds for when the current pricing plan term for this reserved queue expires.\"\n        }\n      ]\n    },\n    \"PurchasedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"purchasedAt\"\n          },\n          \"description\": \"The timestamp in epoch seconds for when you set up the current pricing plan for this reserved queue.\"\n        }\n      ]\n    },\n    \"RenewalType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenewalType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renewalType\"\n          },\n          \"description\": \"Specifies whether the term of your reserved queue pricing plan is automatically extended (AUTO_RENEW) or expires (EXPIRE) at the end of the term.\"\n        }\n      ]\n    },\n    \"ReservedSlots\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservedSlots\"\n          },\n          \"description\": \"Specifies the number of reserved transcode slots (RTS) for this queue. The number of RTS determines how many jobs the queue can process in parallel; each RTS can process one job at a time. When you increase this number, you extend your existing commitment with a new 12-month commitment for a larger number of RTS. The new commitment begins when you purchase the additional capacity. You can't decrease the number of RTS in your reserved queue.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationPlanStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Specifies whether the pricing plan for your reserved queue is ACTIVE\
  \ or EXPIRED.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-reservation-plan-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ReservationPlan
---
