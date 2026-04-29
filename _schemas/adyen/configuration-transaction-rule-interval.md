---
description: TransactionRuleInterval schema from Adyen API
layout: schema
name: TransactionRuleInterval
properties_list:
- description: The day of month, used when the `duration.unit` is **months**. If not provided, by default, this is set to **1**, the first day of the month.
  name: dayOfMonth
  type: integer
- description: 'The day of week, used when the `duration.unit` is **weeks**. If not provided, by default, this is set to **monday**. Possible values: **sunday**, **monday**, **tuesday**, **wednesday**, **thursday**, '
  name: dayOfWeek
  type: string
- description: The duration, which you can specify in hours, days, weeks, or months. The maximum duration is 90 days or an equivalent in other units. Required when the `type` is **rolling** or **sliding**.
  name: duration
  type: object
- description: The time of day, in **hh:mm:ss** format, used when the `duration.unit` is **hours**. If not provided, by default, this is set to **00:00:00**.
  name: timeOfDay
  type: string
- description: The [time zone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones). For example, **Europe/Amsterdam**. By default, this is set to **UTC**.
  name: timeZone
  type: string
- description: 'The [type of interval](https://docs.adyen.com/issuing/transaction-rules#time-intervals) during which the rule conditions and limits apply, and how often counters are reset. Possible values: * **perTra'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transaction-rule-interval-schema.json
slug: configuration-transaction-rule-interval
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-interval-schema.json\",\n  \"title\": \"TransactionRuleInterval\",\n  \"description\": \"TransactionRuleInterval schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dayOfMonth\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The day of month, used when the `duration.unit` is **months**. If not provided, by default, this is set to **1**, the first day of the month.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"dayOfWeek\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The day of week, used when the `duration.unit` is **weeks**. If not provided, by default, this is set to **monday**.\\n\\nPossible values: **sunday**, **monday**, **tuesday**, **wednesday**, **thursday**, **friday**.\",\n     \
  \ \"enum\": [\n        \"friday\",\n        \"monday\",\n        \"saturday\",\n        \"sunday\",\n        \"thursday\",\n        \"tuesday\",\n        \"wednesday\"\n      ],\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The duration, which you can specify in hours, days, weeks, or months. The maximum duration is 90 days or an equivalent in other units. Required when the `type` is **rolling** or **sliding**.\",\n      \"$ref\": \"#/components/schemas/Duration\"\n    },\n    \"timeOfDay\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The time of day, in **hh:mm:ss** format, used when the `duration.unit` is **hours**. If not provided, by default, this is set to **00:00:00**.\",\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The [time zone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones). For example, **Europe/Amsterdam**.\
  \ By default, this is set to **UTC**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The [type of interval](https://docs.adyen.com/issuing/transaction-rules#time-intervals) during which the rule conditions and limits apply, and how often counters are reset.\\n\\nPossible values:\\n  * **perTransaction**: conditions are evaluated and the counters are reset for every transaction.\\n * **daily**: the counters are reset daily at 00:00:00 UTC.\\n * **weekly**: the counters are reset every Monday at 00:00:00 UTC. \\n * **monthly**: the counters reset every first day of the month at 00:00:00 UTC. \\n * **lifetime**: conditions are applied to the lifetime of the payment instrument.\\n * **rolling**: conditions are applied and the counters are reset based on a `duration`. If the reset date and time are not provided, Adyen applies the default reset time similar to fixed intervals.\\nFor example, if the duration is every two weeks, the counter resets every third\
  \ Monday at 00:00:00 UTC.\\n * **sliding**: conditions are applied and the counters are reset based on the current time and a `duration` that you specify.\",\n      \"enum\": [\n        \"daily\",\n        \"lifetime\",\n        \"monthly\",\n        \"perTransaction\",\n        \"rolling\",\n        \"sliding\",\n        \"weekly\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-interval-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRuleInterval
---
