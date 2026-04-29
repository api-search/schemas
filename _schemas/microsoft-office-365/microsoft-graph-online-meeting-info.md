---
description: Details for an attendee to join the meeting online.
layout: schema
name: OnlineMeetingInfo
properties_list:
- description: The URL to join the meeting online.
  name: joinUrl
  type: string
- description: The ID of the conference.
  name: conferenceId
  type: string
- description: The toll number to dial for audio conference.
  name: tollNumber
  type: string
- description: The toll-free numbers to dial.
  name: tollFreeNumbers
  type: array
- description: The pre-formatted quick-dial for this call.
  name: quickDial
  type: string
- description: All phone numbers associated with this conference.
  name: phones
  type: array
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-online-meeting-info-schema.json
slug: microsoft-graph-online-meeting-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OnlineMeetingInfo\",\n  \"type\": \"object\",\n  \"description\": \"Details for an attendee to join the meeting online.\",\n  \"properties\": {\n    \"joinUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to join the meeting online.\"\n    },\n    \"conferenceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the conference.\"\n    },\n    \"tollNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The toll number to dial for audio conference.\"\n    },\n    \"tollFreeNumbers\": {\n      \"type\": \"array\",\n      \"description\": \"The toll-free numbers to dial.\"\n    },\n    \"quickDial\": {\n      \"type\": \"string\",\n      \"description\": \"The pre-formatted quick-dial for this call.\"\n    },\n    \"phones\": {\n      \"type\": \"array\",\n      \"description\": \"All phone numbers associated with this conference.\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-online-meeting-info-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: OnlineMeetingInfo
---
