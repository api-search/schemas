---
description: GetNotificationConfigurationListResponse schema from Adyen API
layout: schema
name: GetNotificationConfigurationListResponse
properties_list:
- description: Details of the notification subscription configurations.
  name: configurations
  type: array
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-get-notification-configuration-list-response-schema.json
slug: notification-configurations-get-notification-configuration-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-get-notification-configuration-list-response-schema.json\",\n  \"title\": \"GetNotificationConfigurationListResponse\",\n  \"description\": \"GetNotificationConfigurationListResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurations\": {\n      \"description\": \"Details of the notification subscription configurations.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/NotificationConfigurationDetails\"\n      },\n      \"type\": \"array\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\
  \n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-get-notification-configuration-list-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetNotificationConfigurationListResponse
---
