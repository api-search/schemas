---
description: A calendar which is a container for events.
layout: schema
name: Calendar
properties_list:
- description: The unique identifier for the calendar.
  name: id
  type: string
- description: The calendar name.
  name: name
  type: string
- description: Specifies the color theme for the calendar.
  name: color
  type: string
- description: Identifies the version of the calendar object.
  name: changeKey
  type: string
- description: Whether the user can write to the calendar.
  name: canEdit
  type: boolean
- description: Whether the user has permission to share the calendar.
  name: canShare
  type: boolean
- description: Whether the user can read calendar items marked as private.
  name: canViewPrivateItems
  type: boolean
- description: Whether this is the default calendar.
  name: isDefaultCalendar
  type: boolean
- description: The calendar color expressed in hex format of three six-digit values.
  name: hexColor
  type: string
- description: Whether the calendar can be deleted from the user's mailbox.
  name: isRemovable
  type: boolean
- description: Whether the calendar supports tracking of meeting responses.
  name: isTallyingResponses
  type: boolean
- description: The online meeting service providers available for events in this calendar.
  name: allowedOnlineMeetingProviders
  type: array
- description: The default online meeting provider for meetings sent from this calendar.
  name: defaultOnlineMeetingProvider
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-calendar-schema.json
slug: microsoft-graph-calendar
source_filename: microsoft-graph-calendar-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Calendar\",\n  \"type\": \"object\",\n  \"description\": \"A calendar which is a container for events.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the calendar.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The calendar name.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the color theme for the calendar.\"\n    },\n    \"changeKey\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the version of the calendar object.\"\n    },\n    \"canEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can write to the calendar.\"\n    },\n    \"canShare\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has permission to share the calendar.\"\n    },\n    \"canViewPrivateItems\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can read calendar items marked as private.\"\n    },\n    \"isDefaultCalendar\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default calendar.\"\n    },\n    \"hexColor\": {\n      \"type\": \"string\",\n      \"description\": \"The calendar color expressed in hex format of three six-digit values.\"\n    },\n    \"isRemovable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the calendar can be deleted from the user's mailbox.\"\n    },\n    \"isTallyingResponses\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the calendar supports tracking of meeting responses.\"\n    },\n    \"allowedOnlineMeetingProviders\": {\n      \"type\": \"array\",\n      \"description\": \"The online meeting service providers available for events in this calendar.\"\n    },\n    \"defaultOnlineMeetingProvider\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The default online meeting provider for meetings sent from this calendar.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-calendar-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: Calendar
---
