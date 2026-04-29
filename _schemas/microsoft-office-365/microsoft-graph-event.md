---
description: An event in a user calendar or the default calendar of a Microsoft 365 group. Contains event details, scheduling, recurrence, attendees, and location information.
layout: schema
name: Event
properties_list:
- description: Unique identifier for the event.
  name: id
  type: string
- description: The text of the event's subject line.
  name: subject
  type: string
- description: A preview of the message associated with the event.
  name: bodyPreview
  type: string
- description: The locations where the event is held or attended from.
  name: locations
  type: array
- description: The collection of attendees for the event.
  name: attendees
  type: array
- description: Set to true if the event lasts all day.
  name: isAllDay
  type: boolean
- description: Set to true if the event has been canceled.
  name: isCancelled
  type: boolean
- description: Set to true if the calendar owner is the organizer.
  name: isOrganizer
  type: boolean
- description: Whether the event is an online meeting.
  name: isOnlineMeeting
  type: boolean
- description: The online meeting service provider.
  name: onlineMeetingProvider
  type: string
- description: A URL for an online meeting.
  name: onlineMeetingUrl
  type: string
- description: The ID for the recurring series master item.
  name: seriesMasterId
  type: string
- description: The event type.
  name: type
  type: string
- description: The status to show.
  name: showAs
  type: string
- description: The importance of the event.
  name: importance
  type: string
- description: The sensitivity of the event.
  name: sensitivity
  type: string
- description: Whether the organizer would like an invitee to send a response.
  name: responseRequested
  type: boolean
- description: Whether new time proposals are allowed for the event.
  name: allowNewTimeProposals
  type: boolean
- description: The categories associated with the event.
  name: categories
  type: array
- description: Whether the event has attachments.
  name: hasAttachments
  type: boolean
- description: A unique identifier across calendars (RFC 2445).
  name: iCalUId
  type: string
- description: The URL to open the event in Outlook on the web.
  name: webLink
  type: string
- description: The date and time the event was created.
  name: createdDateTime
  type: string
- description: The date and time the event was last modified.
  name: lastModifiedDateTime
  type: string
- description: The number of minutes before the event start time for the reminder alert.
  name: reminderMinutesBeforeStart
  type: integer
- description: A custom identifier for the client to avoid redundant POST operations when client retries.
  name: transactionId
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-event-schema.json
slug: microsoft-graph-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Event\",\n  \"type\": \"object\",\n  \"description\": \"An event in a user calendar or the default calendar of a Microsoft 365 group. Contains event details, scheduling, recurrence, attendees, and location information.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the event.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The text of the event's subject line.\"\n    },\n    \"bodyPreview\": {\n      \"type\": \"string\",\n      \"description\": \"A preview of the message associated with the event.\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"description\": \"The locations where the event is held or attended from.\"\n    },\n    \"attendees\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of attendees for the event.\"\n    },\n    \"isAllDay\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true if the event lasts all day.\"\n    },\n    \"isCancelled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true if the event has been canceled.\"\n    },\n    \"isOrganizer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true if the calendar owner is the organizer.\"\n    },\n    \"isOnlineMeeting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event is an online meeting.\"\n    },\n    \"onlineMeetingProvider\": {\n      \"type\": \"string\",\n      \"description\": \"The online meeting service provider.\"\n    },\n    \"onlineMeetingUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A URL for an online meeting.\"\n    },\n    \"seriesMasterId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID for the recurring series master item.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The event type.\"\
  \n    },\n    \"showAs\": {\n      \"type\": \"string\",\n      \"description\": \"The status to show.\"\n    },\n    \"importance\": {\n      \"type\": \"string\",\n      \"description\": \"The importance of the event.\"\n    },\n    \"sensitivity\": {\n      \"type\": \"string\",\n      \"description\": \"The sensitivity of the event.\"\n    },\n    \"responseRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organizer would like an invitee to send a response.\"\n    },\n    \"allowNewTimeProposals\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether new time proposals are allowed for the event.\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"The categories associated with the event.\"\n    },\n    \"hasAttachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event has attachments.\"\n    },\n    \"iCalUId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique\
  \ identifier across calendars (RFC 2445).\"\n    },\n    \"webLink\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to open the event in Outlook on the web.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the event was created.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the event was last modified.\"\n    },\n    \"reminderMinutesBeforeStart\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes before the event start time for the reminder alert.\"\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"A custom identifier for the client to avoid redundant POST operations when client retries.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-event-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: Event
---
