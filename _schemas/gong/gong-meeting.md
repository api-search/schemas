---
description: Represents a meeting in the Gong platform, including scheduling information, participants, and conferencing details.
layout: schema
name: Gong Meeting
properties_list:
- description: Unique meeting identifier.
  name: id
  type: string
- description: Title of the meeting.
  name: title
  type: string
- description: Scheduled start time of the meeting in ISO-8601 format.
  name: scheduledStart
  type: string
- description: Scheduled end time of the meeting in ISO-8601 format.
  name: scheduledEnd
  type: string
- description: Email of the meeting organizer.
  name: organizerEmail
  type: string
- description: URL of the meeting (conferencing link).
  name: meetingUrl
  type: string
- description: Description or agenda for the meeting.
  name: description
  type: string
- description: The meeting provider (e.g., Zoom, Google Meet, Microsoft Teams).
  name: meetingProvider
  type: string
- description: External meeting ID from the conferencing system.
  name: externalMeetingId
  type: string
- description: List of meeting attendees.
  name: attendees
  type: array
provider_name: Gong
provider_slug: gong
schema_file: json-schema/gong-meeting-schema.json
slug: gong-meeting
source_filename: gong-meeting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gong/blob/main/json-schema/gong-meeting-schema.json\",\n  \"title\": \"Gong Meeting\",\n  \"description\": \"Represents a meeting in the Gong platform, including scheduling information, participants, and conferencing details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique meeting identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the meeting.\"\n    },\n    \"scheduledStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled start time of the meeting in ISO-8601 format.\"\n    },\n    \"scheduledEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled end time of the meeting in ISO-8601 format.\"\n    },\n    \"organizerEmail\":\
  \ {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email of the meeting organizer.\"\n    },\n    \"meetingUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the meeting (conferencing link).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description or agenda for the meeting.\"\n    },\n    \"meetingProvider\": {\n      \"type\": \"string\",\n      \"description\": \"The meeting provider (e.g., Zoom, Google Meet, Microsoft Teams).\"\n    },\n    \"externalMeetingId\": {\n      \"type\": \"string\",\n      \"description\": \"External meeting ID from the conferencing system.\"\n    },\n    \"attendees\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MeetingAttendee\"\n      },\n      \"description\": \"List of meeting attendees.\"\n    }\n  },\n  \"required\": [\"id\", \"title\"],\n  \"$defs\": {\n    \"MeetingAttendee\": {\n   \
  \   \"type\": \"object\",\n      \"description\": \"An attendee of a Gong meeting.\",\n      \"properties\": {\n        \"emailAddress\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The attendee's email address.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The attendee's display name.\"\n        },\n        \"responseStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"Accepted\", \"Declined\", \"Tentative\", \"NeedsAction\"],\n          \"description\": \"The attendee's RSVP response status.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/json-schema/gong-meeting-schema.json
tags: []
title: Gong Meeting
---
