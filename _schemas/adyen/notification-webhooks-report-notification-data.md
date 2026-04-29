---
description: ReportNotificationData schema from Adyen API
layout: schema
name: ReportNotificationData
properties_list:
- description: The account holder related to the report.
  name: accountHolder
  type: object
- description: The balance account related to the report.
  name: balanceAccount
  type: object
- description: Unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.
  name: creationDate
  type: string
- description: The URL at which you can download the report. To download, you must authenticate your GET request with your [API credentials](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/overview).
  name: downloadUrl
  type: string
- description: The filename of the report.
  name: fileName
  type: string
- description: Type of report.
  name: reportType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-report-notification-data-schema.json
slug: notification-webhooks-report-notification-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-report-notification-data-schema.json\",\n  \"title\": \"ReportNotificationData\",\n  \"description\": \"ReportNotificationData schema from Adyen API\",\n  \"properties\": {\n    \"accountHolder\": {\n      \"description\": \"The account holder related to the report.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"balanceAccount\": {\n      \"description\": \"The balance account related to the report.\",\n      \"$ref\": \"#/components/schemas/ResourceReference\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"Unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"description\": \"Date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\"\
  ,\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"downloadUrl\": {\n      \"description\": \"The URL at which you can download the report. To download, you must authenticate your GET request with your [API credentials](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/overview).\",\n      \"type\": \"string\"\n    },\n    \"fileName\": {\n      \"description\": \"The filename of the report.\",\n      \"type\": \"string\"\n    },\n    \"reportType\": {\n      \"description\": \"Type of report.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"fileName\",\n    \"reportType\",\n    \"downloadUrl\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-report-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReportNotificationData
---
