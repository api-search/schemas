---
description: Represents a Service Level Objective in Honeycomb, including the SLI query, target percentage, time period, and associated burn alerts for monitoring error budget consumption.
layout: schema
name: Honeycomb SLO
properties_list:
- description: Unique identifier for the SLO.
  name: id
  type: string
- description: The display name of the SLO.
  name: name
  type: string
- description: A human-readable description of what the SLO measures.
  name: description
  type: string
- description: The Service Level Indicator query specification that defines how to measure the SLO.
  name: sli
  type: object
- description: The target percentage for the SLO, such as 99.9 for three nines availability.
  name: target_percentage
  type: number
- description: The rolling time period in days over which the SLO is evaluated.
  name: time_period_days
  type: integer
- description: ISO8601 formatted time the SLO was created.
  name: created_at
  type: string
- description: ISO8601 formatted time the SLO was last updated.
  name: updated_at
  type: string
provider_name: honeycomb
provider_slug: honeycomb
schema_file: json-schema/honeycomb-slo-schema.json
slug: honeycomb-slo
source_filename: honeycomb-slo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://honeycomb.io/schemas/honeycomb/slo.json\",\n  \"title\": \"Honeycomb SLO\",\n  \"description\": \"Represents a Service Level Objective in Honeycomb, including the SLI query, target percentage, time period, and associated burn alerts for monitoring error budget consumption.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"sli\", \"target_percentage\", \"time_period_days\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the SLO.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 200,\n      \"description\": \"The display name of the SLO.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of what the SLO measures.\"\n    },\n    \"sli\": {\n      \"type\": \"object\",\n      \"description\": \"The\
  \ Service Level Indicator query specification that defines how to measure the SLO.\"\n    },\n    \"target_percentage\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"The target percentage for the SLO, such as 99.9 for three nines availability.\"\n    },\n    \"time_period_days\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The rolling time period in days over which the SLO is evaluated.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO8601 formatted time the SLO was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO8601 formatted time the SLO was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"BurnAlert\": {\n      \"type\": \"object\",\n      \"description\": \"A burn alert that notifies recipients when the SLO error budget is being\
  \ consumed too quickly.\",\n      \"required\": [\"slo_id\", \"alert_type\", \"recipients\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the burn alert.\"\n        },\n        \"slo_id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the SLO this burn alert monitors.\"\n        },\n        \"alert_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of burn alert.\",\n          \"enum\": [\"budget_rate\", \"exhaustion_time\"]\n        },\n        \"exhaustion_minutes\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"For exhaustion_time alerts, the number of minutes before budget exhaustion that triggers the alert.\"\n        },\n        \"budget_rate_window_minutes\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"For budget_rate alerts, the window in minutes\
  \ over which to measure the burn rate.\"\n        },\n        \"budget_rate_decrease_percent\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"For budget_rate alerts, the percentage decrease in budget that triggers the alert.\"\n        },\n        \"recipients\": {\n          \"type\": \"array\",\n          \"description\": \"List of recipients to notify when the burn alert fires.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/RecipientRef\"\n          }\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO8601 formatted time the burn alert was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO8601 formatted time the burn alert was last updated.\"\n        }\n      }\n    },\n    \"RecipientRef\": {\n      \"\
  type\": \"object\",\n      \"description\": \"A reference to a notification recipient.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the recipient to notify.\"\n        }\n      }\n    },\n    \"SLOReport\": {\n      \"type\": \"object\",\n      \"description\": \"Historical SLO performance report data.\",\n      \"properties\": {\n        \"slo_id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the SLO this report is for.\"\n        },\n        \"budget_remaining\": {\n          \"type\": \"number\",\n          \"description\": \"The remaining error budget as a percentage.\"\n        },\n        \"budget_used\": {\n          \"type\": \"number\",\n          \"description\": \"The used error budget as a percentage.\"\n        },\n        \"compliance\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n        \
  \  \"description\": \"The current compliance percentage.\"\n        },\n        \"time_period_days\": {\n          \"type\": \"integer\",\n          \"description\": \"The time period in days for the report.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/json-schema/honeycomb-slo-schema.json
tags: []
title: Honeycomb SLO
---
