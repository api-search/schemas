---
description: Details about the pricing plan for your reserved queue. Required for reserved queues and not applicable to on-demand queues.
layout: schema
name: ReservationPlanSettings
properties_list:
- description: ''
  name: Commitment
  type: object
- description: ''
  name: RenewalType
  type: object
- description: ''
  name: ReservedSlots
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-reservation-plan-settings-schema.json
slug: mediaconvert-api-reservation-plan-settings
source_filename: mediaconvert-api-reservation-plan-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-reservation-plan-settings-schema.json\",\n  \"title\": \"ReservationPlanSettings\",\n  \"description\": \"Details about the pricing plan for your reserved queue. Required for reserved queues and not applicable to on-demand queues.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Commitment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Commitment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"commitment\"\n          },\n          \"description\": \"The length of the term of your reserved queue pricing plan commitment.\"\n        }\n      ]\n    },\n    \"RenewalType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenewalType\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"renewalType\"\n          },\n          \"description\": \"Specifies whether the term of your reserved queue pricing plan is automatically extended (AUTO_RENEW) or expires (EXPIRE) at the end of the term. When your term is auto renewed, you extend your commitment by 12 months from the auto renew date. You can cancel this commitment.\"\n        }\n      ]\n    },\n    \"ReservedSlots\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservedSlots\"\n          },\n          \"description\": \"Specifies the number of reserved transcode slots (RTS) for this queue. The number of RTS determines how many jobs the queue can process in parallel; each RTS can process one job at a time. You can't decrease the number of RTS in your reserved queue. You can increase the number of RTS by extending your existing commitment with a new 12-month commitment for the larger number. The new\
  \ commitment begins when you purchase the additional capacity. You can't cancel your commitment or revert to your original commitment after you increase the capacity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Commitment\",\n    \"ReservedSlots\",\n    \"RenewalType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-reservation-plan-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ReservationPlanSettings
---
