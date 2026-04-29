---
description: An event type defines a kind of meeting that can be scheduled through Calendly, including its name, duration, location configuration, custom questions, and availability settings.
layout: schema
name: Calendly Event Type
properties_list:
- description: The canonical URI of the event type resource.
  name: uri
  type: string
- description: The name of the event type displayed to invitees.
  name: name
  type: string
- description: Whether the event type is currently active and available for scheduling.
  name: active
  type: boolean
- description: The booking method for the event type.
  name: booking_method
  type: string
- description: The URL-friendly slug for the event type.
  name: slug
  type: string
- description: The public URL of the event type's scheduling page.
  name: scheduling_url
  type: string
- description: The default duration of the event in minutes.
  name: duration
  type: integer
- description: Whether the event type is for one-on-one or group meetings.
  name: kind
  type: string
- description: For team event types, the strategy for assigning hosts to meetings.
  name: pooling_type
  type:
  - string
  - 'null'
- description: The type classification of the event type.
  name: type
  type: string
- description: The hex color code associated with the event type for display purposes.
  name: color
  type: string
- description: The plain text description of the event type.
  name: description_plain
  type:
  - string
  - 'null'
- description: The HTML-formatted description of the event type.
  name: description_html
  type:
  - string
  - 'null'
- description: An internal note visible only to the event host, not shown to invitees.
  name: internal_note
  type:
  - string
  - 'null'
- description: ''
  name: profile
  type: object
- description: Whether the event type is hidden from the user's public scheduling page.
  name: secret
  type: boolean
- description: The timestamp when the event type was deleted, if applicable.
  name: deleted_at
  type:
  - string
  - 'null'
- description: Custom questions displayed on the booking page for invitees to answer.
  name: custom_questions
  type: array
- description: The timestamp when the event type was created.
  name: created_at
  type: string
- description: The timestamp when the event type was last updated.
  name: updated_at
  type: string
provider_name: Calendly
provider_slug: calendly
schema_file: json-schema/calendly-event-type-schema.json
slug: calendly-event-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.calendly.com/schemas/calendly/event-type.json\",\n  \"title\": \"Calendly Event Type\",\n  \"description\": \"An event type defines a kind of meeting that can be scheduled through Calendly, including its name, duration, location configuration, custom questions, and availability settings.\",\n  \"type\": \"object\",\n  \"required\": [\"uri\", \"name\", \"active\", \"duration\", \"scheduling_url\"],\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The canonical URI of the event type resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event type displayed to invitees.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event type is currently active and available for scheduling.\"\n    },\n    \"booking_method\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"instant\", \"poll\"],\n      \"description\": \"The booking method for the event type.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug for the event type.\"\n    },\n    \"scheduling_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The public URL of the event type's scheduling page.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"The default duration of the event in minutes.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\"solo\", \"group\"],\n      \"description\": \"Whether the event type is for one-on-one or group meetings.\"\n    },\n    \"pooling_type\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [\"round_robin\", \"collective\", null],\n      \"description\": \"For team event types, the strategy for assigning hosts to meetings.\"\
  \n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"StandardEventType\", \"AdhocEventType\"],\n      \"description\": \"The type classification of the event type.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"pattern\": \"^#[0-9a-fA-F]{6}$\",\n      \"description\": \"The hex color code associated with the event type for display purposes.\"\n    },\n    \"description_plain\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The plain text description of the event type.\"\n    },\n    \"description_html\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The HTML-formatted description of the event type.\"\n    },\n    \"internal_note\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An internal note visible only to the event host, not shown to invitees.\"\n    },\n    \"profile\": {\n      \"$ref\": \"#/$defs/Profile\"\n    },\n    \"secret\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether the event type is hidden from the user's public scheduling page.\"\n    },\n    \"deleted_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the event type was deleted, if applicable.\"\n    },\n    \"custom_questions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomQuestion\"\n      },\n      \"description\": \"Custom questions displayed on the booking page for invitees to answer.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the event type was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the event type was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Profile\": {\n      \"type\": \"object\",\n      \"description\": \"The profile (user or team)\
  \ associated with the event type.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Team\"],\n          \"description\": \"The type of profile that owns the event type.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the profile owner.\"\n        },\n        \"owner\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URI of the profile owner (user or organization).\"\n        }\n      }\n    },\n    \"CustomQuestion\": {\n      \"type\": \"object\",\n      \"description\": \"A custom question displayed on the event type booking page.\",\n      \"required\": [\"uuid\", \"name\", \"type\", \"enabled\", \"required\"],\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n          \"description\": \"The UUID of the custom question.\"\n        },\n        \"name\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The text of the question displayed to invitees.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"string\", \"text\", \"phone_number\", \"single_select\", \"multi_select\"],\n          \"description\": \"The type of input expected for the answer.\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The display order of the question on the booking page.\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the question is currently enabled and visible.\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the invitee must provide an answer to proceed with booking.\"\n        },\n        \"answer_choices\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n   \
  \       \"description\": \"The available answer choices for single_select and multi_select questions.\"\n        },\n        \"include_other\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether an 'Other' free-text option is included for select-type questions.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/json-schema/calendly-event-type-schema.json
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
title: Calendly Event Type
---
