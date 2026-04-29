---
description: It conveys Information related to the event, and possible action (maintenance, message to display). Content of the EventNotification message.
layout: schema
name: EventNotification
properties_list:
- description: Date and time of a transaction for the Sale System, the POI System or the Acquirer.
  name: TimeStamp
  type: string
- description: ''
  name: EventToNotify
  type: object
- description: If present, the Sale logs it for further examination.
  name: EventDetails
  type: string
- description: Mandatory if EventToNotify is Reject, absent in other cases.
  name: RejectedMessage
  type: string
- description: Indicates if the occurred event requires maintenance call or action.
  name: MaintenanceRequiredFlag
  type: boolean
- description: If the language is selected by the Sale System before the request to the POI.
  name: CustomerLanguage
  type: string
- description: ''
  name: DisplayOutput
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-event-notification-schema.json
slug: terminal-event-notification
source_filename: terminal-event-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-event-notification-schema.json\",\n  \"title\": \"EventNotification\",\n  \"description\": \"It conveys Information related to the event, and possible action (maintenance, message to display). Content of the EventNotification message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeStamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of a transaction for the Sale System, the POI System or the Acquirer.\"\n    },\n    \"EventToNotify\": {\n      \"$ref\": \"#/components/schemas/EventToNotify\"\n    },\n    \"EventDetails\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If present, the Sale logs it for further examination.\"\n    },\n    \"RejectedMessage\": {\n      \"type\": \"string\",\n  \
  \    \"format\": \"byte\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"Mandatory if EventToNotify is Reject, absent in other cases.\"\n    },\n    \"MaintenanceRequiredFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Indicates if the occurred event requires maintenance call or action.\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"If the language is selected by the Sale System before the request to the POI.\"\n    },\n    \"DisplayOutput\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DisplayOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"TimeStamp\",\n    \"EventToNotify\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-event-notification-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EventNotification
---
