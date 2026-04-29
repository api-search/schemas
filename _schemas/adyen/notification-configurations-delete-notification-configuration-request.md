---
description: DeleteNotificationConfigurationRequest schema from Adyen API
layout: schema
name: DeleteNotificationConfigurationRequest
properties_list:
- description: A list of IDs of the notification subscription configurations to be deleted.
  name: notificationIds
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-delete-notification-configuration-request-schema.json
slug: notification-configurations-delete-notification-configuration-request
source_filename: notification-configurations-delete-notification-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-delete-notification-configuration-request-schema.json\",\n  \"title\": \"DeleteNotificationConfigurationRequest\",\n  \"description\": \"DeleteNotificationConfigurationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationIds\": {\n      \"description\": \"A list of IDs of the notification subscription configurations to be deleted.\",\n      \"items\": {\n        \"format\": \"int64\",\n        \"type\": \"integer\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"notificationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-delete-notification-configuration-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeleteNotificationConfigurationRequest
---
