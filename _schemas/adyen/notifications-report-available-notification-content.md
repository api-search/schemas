---
description: ReportAvailableNotificationContent schema from Adyen API
layout: schema
name: ReportAvailableNotificationContent
properties_list:
- description: The code of the Account to which the report applies.
  name: accountCode
  type: string
- description: The type of Account to which the report applies.
  name: accountType
  type: string
- description: The date of the event to which the report applies.
  name: eventDate
  type: string
- description: The URL at which the report can be accessed.
  name: remoteAccessUrl
  type: string
- description: Indicates whether the event resulted in a success.
  name: success
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-report-available-notification-content-schema.json
slug: notifications-report-available-notification-content
source_filename: notifications-report-available-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-report-available-notification-content-schema.json\",\n  \"title\": \"ReportAvailableNotificationContent\",\n  \"description\": \"ReportAvailableNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the Account to which the report applies.\",\n      \"type\": \"string\"\n    },\n    \"accountType\": {\n      \"description\": \"The type of Account to which the report applies.\",\n      \"type\": \"string\"\n    },\n    \"eventDate\": {\n      \"description\": \"The date of the event to which the report applies.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"remoteAccessUrl\": {\n      \"description\": \"The URL at which the report can be accessed.\",\n      \"type\": \"\
  string\"\n    },\n    \"success\": {\n      \"description\": \"Indicates whether the event resulted in a success.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-report-available-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReportAvailableNotificationContent
---
