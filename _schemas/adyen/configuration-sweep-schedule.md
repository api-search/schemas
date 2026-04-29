---
description: SweepSchedule schema from Adyen API
layout: schema
name: SweepSchedule
properties_list:
- description: A [cron expression](https://en.wikipedia.org/wiki/Cron#CRON_expression) that is used to set the sweep schedule. The schedule uses the time zone of the balance account. For example, **30 17 * * MON** s
  name: cronExpression
  type: string
- description: 'The schedule type. Possible values: * **cron**: push out funds based on a `cronExpression`. * **daily**: push out funds daily at 07:00 AM CET. * **weekly**: push out funds every Monday at 07:00 AM CET'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-sweep-schedule-schema.json
slug: configuration-sweep-schedule
source_filename: configuration-sweep-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-sweep-schedule-schema.json\",\n  \"title\": \"SweepSchedule\",\n  \"description\": \"SweepSchedule schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cronExpression\": {\n      \"description\": \"A [cron expression](https://en.wikipedia.org/wiki/Cron#CRON_expression) that is used to set the sweep schedule. The schedule uses the time zone of the balance account. \\nFor example, **30 17 * * MON** schedules a sweep every Monday at 17:30.\\n\\nThe expression must have five values separated by a single space in the following order:\\n\\n* Minute: **0-59**\\n\\n* Hour: **0-23**\\n\\n* Day of the month: **1-31**\\n\\n* Month: **1-12** or **JAN-DEC**\\n\\n* Day of the week: **0-7** (0 and 7 are Sunday) or **MON-SUN**.\\n\\nThe following non-standard characters are supported: **&ast;**,\
  \ **L**, **#**, **W** and **/**. See [crontab guru](https://crontab.guru/) for more examples.\\n\\nRequired when `type` is **cron**.\\n\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The schedule type.\\n\\nPossible values:\\n\\n* **cron**: push out funds based on a `cronExpression`.\\n\\n* **daily**: push out funds daily at 07:00 AM CET.\\n\\n* **weekly**: push out funds every Monday at 07:00 AM CET.\\n\\n* **monthly**: push out funds every first of the month at 07:00 AM CET.\\n\\n* **balance**: pull in funds instantly if the balance is less than or equal to the `triggerAmount`.\\nYou can only use this for sweeps of `type` **pull** and when the source is a `merchantAccount` or `transferInstrument`.\\nIf the source is transferInstrument, merchant account identifier is still required, with which you want to process the transaction.\\n\",\n      \"enum\": [\n        \"daily\",\n        \"weekly\",\n        \"monthly\",\n        \"balance\",\n        \"\
  cron\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-sweep-schedule-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepSchedule
---
