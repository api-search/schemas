---
description: GetNotificationConfigurationResponse schema from Adyen API
layout: schema
name: GetNotificationConfigurationResponse
properties_list:
- description: Details of the notification subscription configuration.
  name: configurationDetails
  type: object
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
schema_file: json-schema/notification-configurations-get-notification-configuration-response-schema.json
slug: notification-configurations-get-notification-configuration-response
source_filename: notification-configurations-get-notification-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-get-notification-configuration-response-schema.json\",\n  \"title\": \"GetNotificationConfigurationResponse\",\n  \"description\": \"GetNotificationConfigurationResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationDetails\": {\n      \"description\": \"Details of the notification subscription configuration.\",\n      \"$ref\": \"#/components/schemas/NotificationConfigurationDetails\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The\
  \ reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"configurationDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-get-notification-configuration-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetNotificationConfigurationResponse
---
