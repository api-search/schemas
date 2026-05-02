---
description: Represents a calendar container for event resources as exposed through the Microsoft Graph Calendar API. Can be a calendar for a user or the default calendar of a Microsoft 365 group. Users can organize calendars in calendar groups.
layout: schema
name: Microsoft Exchange Calendar
properties_list:
- description: The calendar's unique identifier
  name: id
  type: string
- description: The calendar name
  name: name
  type: string
- description: Specifies the color theme to distinguish the calendar in the UI
  name: color
  type: string
- description: 'The calendar color in hex format (e.g. #FF0000)'
  name: hexColor
  type: string
- description: Whether this is the default calendar for new events
  name: isDefaultCalendar
  type: boolean
- description: Identifies the version of the calendar object
  name: changeKey
  type: string
- description: Whether the user can write to the calendar
  name: canEdit
  type: boolean
- description: Whether the user has permission to share the calendar
  name: canShare
  type: boolean
- description: Whether the user can read private calendar items
  name: canViewPrivateItems
  type: boolean
- description: Whether this calendar can be deleted from the mailbox
  name: isRemovable
  type: boolean
- description: Whether this calendar supports tracking of meeting responses
  name: isTallyingResponses
  type: boolean
- description: The user who created or added the calendar
  name: owner
  type: object
- description: Online meeting providers available for this calendar
  name: allowedOnlineMeetingProviders
  type: array
- description: Default online meeting provider for meetings from this calendar
  name: defaultOnlineMeetingProvider
  type: string
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schema_file: json-schema/microsoft-exchange-calendar-schema.json
slug: microsoft-exchange-calendar
source_filename: microsoft-exchange-calendar-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-exchange/json-schema/microsoft-exchange-calendar-schema.json\",\n  \"title\": \"Microsoft Exchange Calendar\",\n  \"description\": \"Represents a calendar container for event resources as exposed through the Microsoft Graph Calendar API. Can be a calendar for a user or the default calendar of a Microsoft 365 group. Users can organize calendars in calendar groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The calendar's unique identifier\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The calendar name\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"auto\",\n        \"lightBlue\",\n        \"lightGreen\",\n        \"lightOrange\",\n        \"lightGray\",\n        \"lightYellow\"\
  ,\n        \"lightTeal\",\n        \"lightPink\",\n        \"lightBrown\",\n        \"lightRed\",\n        \"maxColor\"\n      ],\n      \"description\": \"Specifies the color theme to distinguish the calendar in the UI\"\n    },\n    \"hexColor\": {\n      \"type\": \"string\",\n      \"pattern\": \"^#?[0-9a-fA-F]{6}$\",\n      \"description\": \"The calendar color in hex format (e.g. #FF0000)\",\n      \"readOnly\": true\n    },\n    \"isDefaultCalendar\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default calendar for new events\"\n    },\n    \"changeKey\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the version of the calendar object\",\n      \"readOnly\": true\n    },\n    \"canEdit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can write to the calendar\",\n      \"readOnly\": true\n    },\n    \"canShare\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has permission\
  \ to share the calendar\",\n      \"readOnly\": true\n    },\n    \"canViewPrivateItems\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user can read private calendar items\",\n      \"readOnly\": true\n    },\n    \"isRemovable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this calendar can be deleted from the mailbox\",\n      \"readOnly\": true\n    },\n    \"isTallyingResponses\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this calendar supports tracking of meeting responses\",\n      \"readOnly\": true\n    },\n    \"owner\": {\n      \"$ref\": \"#/$defs/emailAddress\",\n      \"description\": \"The user who created or added the calendar\"\n    },\n    \"allowedOnlineMeetingProviders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"unknown\", \"skypeForBusiness\", \"skypeForConsumer\", \"teamsForBusiness\"]\n      },\n      \"description\": \"Online meeting\
  \ providers available for this calendar\"\n    },\n    \"defaultOnlineMeetingProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown\", \"skypeForBusiness\", \"skypeForConsumer\", \"teamsForBusiness\"],\n      \"description\": \"Default online meeting provider for meetings from this calendar\"\n    }\n  },\n  \"$defs\": {\n    \"emailAddress\": {\n      \"type\": \"object\",\n      \"description\": \"The name and email address of a person\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/json-schema/microsoft-exchange-calendar-schema.json
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
title: Microsoft Exchange Calendar
---
