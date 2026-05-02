---
description: Represents a trigger alerting rule in Honeycomb that fires when query results meet specified threshold conditions, notifying configured recipients via PagerDuty, Email, Webhook, Microsoft Teams, or Slack.
layout: schema
name: Honeycomb Trigger
properties_list:
- description: Unique identifier for the trigger.
  name: id
  type: string
- description: The display name of the trigger.
  name: name
  type: string
- description: A human-readable description of what the trigger monitors.
  name: description
  type: string
- description: Whether the trigger is currently disabled.
  name: disabled
  type: boolean
- description: The query specification that defines the data to evaluate.
  name: query
  type: object
- description: ''
  name: threshold
  type: object
- description: How frequently in seconds the trigger is evaluated.
  name: frequency
  type: integer
- description: List of recipients to notify when the trigger fires.
  name: recipients
  type: array
- description: ISO8601 formatted time the trigger was created.
  name: created_at
  type: string
- description: ISO8601 formatted time the trigger was last updated.
  name: updated_at
  type: string
provider_name: honeycomb
provider_slug: honeycomb
schema_file: json-schema/honeycomb-trigger-schema.json
slug: honeycomb-trigger
source_filename: honeycomb-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://honeycomb.io/schemas/honeycomb/trigger.json\",\n  \"title\": \"Honeycomb Trigger\",\n  \"description\": \"Represents a trigger alerting rule in Honeycomb that fires when query results meet specified threshold conditions, notifying configured recipients via PagerDuty, Email, Webhook, Microsoft Teams, or Slack.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"query\", \"threshold\", \"recipients\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the trigger.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"The display name of the trigger.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of what the trigger monitors.\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the trigger is currently disabled.\"\n    },\n    \"query\": {\n      \"type\": \"object\",\n      \"description\": \"The query specification that defines the data to evaluate.\"\n    },\n    \"threshold\": {\n      \"$ref\": \"#/$defs/Threshold\"\n    },\n    \"frequency\": {\n      \"type\": \"integer\",\n      \"minimum\": 60,\n      \"description\": \"How frequently in seconds the trigger is evaluated.\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"description\": \"List of recipients to notify when the trigger fires.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/RecipientRef\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO8601 formatted time the trigger was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO8601 formatted time the trigger was last updated.\"\
  \n    }\n  },\n  \"$defs\": {\n    \"Threshold\": {\n      \"type\": \"object\",\n      \"description\": \"The threshold configuration that determines when the trigger fires.\",\n      \"required\": [\"op\", \"value\"],\n      \"properties\": {\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator for the threshold.\",\n          \"enum\": [\">\", \">=\", \"<\", \"<=\"]\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"The threshold value to compare against.\"\n        },\n        \"exceeded_limit\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Number of consecutive times the threshold must be exceeded before the trigger fires.\"\n        }\n      }\n    },\n    \"RecipientRef\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a notification recipient.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n     \
  \   \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the recipient to notify.\"\n        }\n      }\n    },\n    \"Recipient\": {\n      \"type\": \"object\",\n      \"description\": \"A notification recipient that can be targeted by triggers and burn alerts.\",\n      \"required\": [\"type\", \"target\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the recipient.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The notification channel type.\",\n          \"enum\": [\"email\", \"pagerduty\", \"slack\", \"webhook\", \"msteams\"]\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"The target address or identifier for the recipient, such as an email address or webhook URL.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  ,\n          \"description\": \"ISO8601 formatted time the recipient was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO8601 formatted time the recipient was last updated.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/honeycomb/refs/heads/main/json-schema/honeycomb-trigger-schema.json
tags: []
title: Honeycomb Trigger
---
