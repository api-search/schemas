---
description: A scheduled event represents a booked meeting in Calendly with a specific start time, end time, location, host memberships, and associated invitees.
layout: schema
name: Calendly Scheduled Event
properties_list:
- description: The canonical URI of the scheduled event resource.
  name: uri
  type: string
- description: The name of the scheduled event, inherited from the event type.
  name: name
  type: string
- description: The current status of the scheduled event.
  name: status
  type: string
- description: The start time of the event in UTC (ISO 8601 format).
  name: start_time
  type: string
- description: The end time of the event in UTC (ISO 8601 format).
  name: end_time
  type: string
- description: The URI of the event type this event was created from.
  name: event_type
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: invitees_counter
  type: object
- description: ''
  name: cancellation
  type: object
- description: The list of users who are members (hosts) of this event.
  name: event_memberships
  type: array
- description: Additional guests invited to the event beyond the primary invitee.
  name: event_guests
  type: array
- description: The timestamp when the event was created.
  name: created_at
  type: string
- description: The timestamp when the event was last updated.
  name: updated_at
  type: string
provider_name: Calendly
provider_slug: calendly
schema_file: json-schema/calendly-scheduled-event-schema.json
slug: calendly-scheduled-event
source_filename: calendly-scheduled-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.calendly.com/schemas/calendly/scheduled-event.json\",\n  \"title\": \"Calendly Scheduled Event\",\n  \"description\": \"A scheduled event represents a booked meeting in Calendly with a specific start time, end time, location, host memberships, and associated invitees.\",\n  \"type\": \"object\",\n  \"required\": [\"uri\", \"name\", \"status\", \"start_time\", \"end_time\", \"event_type\"],\n  \"properties\": {\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The canonical URI of the scheduled event resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the scheduled event, inherited from the event type.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"canceled\"],\n      \"description\": \"The current status of the scheduled event.\"\n  \
  \  },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time of the event in UTC (ISO 8601 format).\"\n    },\n    \"end_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end time of the event in UTC (ISO 8601 format).\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URI of the event type this event was created from.\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/Location\"\n    },\n    \"invitees_counter\": {\n      \"$ref\": \"#/$defs/InviteesCounter\"\n    },\n    \"cancellation\": {\n      \"$ref\": \"#/$defs/Cancellation\"\n    },\n    \"event_memberships\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EventMembership\"\n      },\n      \"description\": \"The list of users who are members (hosts) of this event.\"\n    },\n    \"event_guests\":\
  \ {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EventGuest\"\n      },\n      \"description\": \"Additional guests invited to the event beyond the primary invitee.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the event was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the event was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\": \"The location configuration for a scheduled event, specifying where the meeting takes place.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of location.\",\n          \"enum\": [\n            \"physical\",\n            \"outbound_call\",\n            \"inbound_call\",\n            \"google_conference\"\
  ,\n            \"zoom\",\n            \"gotomeeting\",\n            \"microsoft_teams_conference\",\n            \"webex_conference\",\n            \"custom\"\n          ]\n        },\n        \"location\": {\n          \"type\": \"string\",\n          \"description\": \"The location details such as a physical address, phone number, or custom location string.\"\n        },\n        \"join_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL to join the meeting for virtual conference locations.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of conference link generation (e.g., initiated, processing, pushed, failed).\"\n        },\n        \"additional_info\": {\n          \"type\": \"string\",\n          \"description\": \"Additional information about the location provided by the host.\"\n        }\n      }\n    },\n    \"InviteesCounter\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A count of invitees by status for the scheduled event.\",\n      \"properties\": {\n        \"total\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The total number of invitees.\"\n        },\n        \"active\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of active (non-canceled) invitees.\"\n        },\n        \"limit\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The maximum number of invitees allowed for the event.\"\n        }\n      }\n    },\n    \"Cancellation\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the cancellation of an event or invitee.\",\n      \"properties\": {\n        \"canceled_by\": {\n          \"type\": \"string\",\n          \"description\": \"The name or identifier of the person who canceled.\"\n        },\n        \"reason\": {\n          \"type\"\
  : \"string\",\n          \"maxLength\": 10000,\n          \"description\": \"The reason provided for the cancellation.\"\n        },\n        \"canceler_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"host\", \"invitee\"],\n          \"description\": \"Whether the host or the invitee canceled the event.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp when the cancellation occurred.\"\n        }\n      }\n    },\n    \"EventMembership\": {\n      \"type\": \"object\",\n      \"description\": \"A user who is a member (host) of a scheduled event.\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URI of the user who is a host of the event.\"\n        },\n        \"user_email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\"\
  : \"The email address of the event host.\"\n        },\n        \"user_name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the event host.\"\n        }\n      }\n    },\n    \"EventGuest\": {\n      \"type\": \"object\",\n      \"description\": \"An additional guest invited to a scheduled event.\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the guest.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the guest was added to the event.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the guest record was last updated.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/json-schema/calendly-scheduled-event-schema.json
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
title: Calendly Scheduled Event
---
