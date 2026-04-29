---
description: SweepSchedule schema from Adyen API
layout: schema
name: SweepSchedule
properties_list:
- description: 'The schedule type. Possible values: * **cron**: push out funds based on a cron expression. * **daily**: push out funds daily at 07:00 AM CET. * **weekly**: push out funds every Monday at 07:00 AM CET.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-sweep-schedule-schema.json
slug: notification-webhooks-sweep-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-schedule-schema.json\",\n  \"title\": \"SweepSchedule\",\n  \"description\": \"SweepSchedule schema from Adyen API\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"The schedule type.\\n\\nPossible values:\\n\\n* **cron**: push out funds based on a cron expression.\\n\\n* **daily**: push out funds daily at 07:00 AM CET.\\n\\n* **weekly**: push out funds every Monday at 07:00 AM CET.\\n\\n* **monthly**: push out funds every first of the month at 07:00 AM CET.\\n\\n* **balance**: pull in funds instantly if the balance is less than or equal to the `triggerAmount`. You can only use this for sweeps of `type` **pull** and when the source is a `merchantAccount` or `transferInstrument`.\",\n      \"enum\": [\n        \"daily\",\n        \"weekly\",\n        \"monthly\",\n   \
  \     \"balance\",\n        \"cron\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false,\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-schedule-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepSchedule
---
