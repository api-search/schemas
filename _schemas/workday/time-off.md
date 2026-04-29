---
description: Represents time-off data for a worker in Workday, including time-off requests, entries, balances, and leave of absence records.
layout: schema
name: Time Off
properties_list:
- description: The Workday ID of the time-off record.
  name: id
  type: string
- description: A display descriptor for the time-off record.
  name: descriptor
  type: string
- description: The worker this time-off record belongs to.
  name: worker
  type: object
- description: The type of time off (e.g., Vacation, Sick, Personal).
  name: timeOffType
  type: object
- description: Individual time-off entries (one per day).
  name: timeOffEntries
  type: array
- description: The status of the time-off request.
  name: status
  type: string
- description: The total quantity of time off requested.
  name: totalQuantity
  type: number
- description: The unit of measure for time off (e.g., Hours, Days).
  name: unit
  type: string
- description: A comment or reason for the time-off request.
  name: comment
  type: string
- description: When the time-off request was submitted.
  name: requestedDate
  type: string
- description: Time-off plan balances for the worker.
  name: balances
  type: array
- description: Leave of absence details, if applicable.
  name: leaveOfAbsence
  type: object
- description: A link to the full time-off resource.
  name: href
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/time-off.json
slug: time-off
source_filename: time-off.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://workday.com/schemas/time-off.json\",\n  \"title\": \"Time Off\",\n  \"description\": \"Represents time-off data for a worker in Workday, including time-off requests, entries, balances, and leave of absence records.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the time-off record.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the time-off record.\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The worker this time-off record belongs to.\"\n    },\n    \"timeOffType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The type of time off (e.g., Vacation, Sick, Personal).\"\n    },\n    \"timeOffEntries\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Individual time-off entries (one per day).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TimeOffEntry\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the time-off request.\",\n      \"enum\": [\"Requested\", \"Approved\", \"Denied\", \"Cancelled\", \"In Progress\"]\n    },\n    \"totalQuantity\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The total quantity of time off requested.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measure for time off (e.g., Hours, Days).\",\n      \"enum\": [\"Hours\", \"Days\"]\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A comment or reason for the time-off request.\"\n    },\n    \"requestedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the time-off request was submitted.\"\n    },\n    \"balances\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"Time-off plan balances for the worker.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TimeOffBalance\"\n      }\n    },\n    \"leaveOfAbsence\": {\n      \"$ref\": \"#/$defs/LeaveOfAbsence\",\n      \"description\": \"Leave of absence details, if applicable.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A link to the full time-off resource.\"\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"TimeOffEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A single day's time-off entry.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the entry.\"\n        },\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The date of the time off.\"\n        },\n        \"dailyQuantity\": {\n          \"type\": \"number\"\
  ,\n          \"format\": \"double\",\n          \"description\": \"The quantity of time off for the day.\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"description\": \"The unit of measurement (Hours or Days).\"\n        },\n        \"timeOffType\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The time-off type for this entry.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the entry.\"\n        },\n        \"comment\": {\n          \"type\": \"string\",\n          \"description\": \"A comment for this specific day.\"\n        }\n      }\n    },\n    \"TimeOffBalance\": {\n      \"type\": \"object\",\n      \"description\": \"A time-off plan balance for a worker.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the balance record.\"\n        },\n        \"descriptor\": {\n\
  \          \"type\": \"string\"\n        },\n        \"timeOffPlan\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The time-off plan.\"\n        },\n        \"balance\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"The current balance amount.\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"description\": \"The unit of the balance (Hours or Days).\"\n        },\n        \"asOfDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The effective date of the balance.\"\n        },\n        \"accrued\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Total time off accrued.\"\n        },\n        \"used\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Total time off used.\"\n        },\n        \"scheduled\": {\n\
  \          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Total time off scheduled but not yet taken.\"\n        },\n        \"carryover\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Carryover from previous period.\"\n        }\n      }\n    },\n    \"LeaveOfAbsence\": {\n      \"type\": \"object\",\n      \"description\": \"A leave of absence record.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"leaveType\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The type of leave (e.g., FMLA, Parental, Medical, Personal).\"\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The start date of the leave.\"\n        },\n        \"estimatedEndDate\": {\n    \
  \      \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"The estimated end date of the leave.\"\n        },\n        \"actualEndDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"The actual end date of the leave.\"\n        },\n        \"lastDayOfWork\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The last day of work before the leave.\"\n        },\n        \"firstDayBackAtWork\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"The first day back at work after the leave.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the leave of absence.\",\n          \"enum\": [\"Requested\", \"Approved\", \"In Progress\", \"Completed\", \"Cancelled\"]\n        },\n        \"reason\": {\n          \"$ref\":\
  \ \"#/$defs/ResourceReference\",\n          \"description\": \"The reason for the leave of absence.\"\n        }\n      }\n    },\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Workday resource.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the referenced resource.\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"A display descriptor for the referenced resource.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A link to the referenced resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/time-off.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Time Off
---
