---
description: GetNotificationConfigurationRequest schema from Adyen API
layout: schema
name: GetNotificationConfigurationRequest
properties_list:
- description: The ID of the notification subscription configuration whose details are to be retrieved.
  name: notificationId
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-get-notification-configuration-request-schema.json
slug: notification-configurations-get-notification-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-get-notification-configuration-request-schema.json\",\n  \"title\": \"GetNotificationConfigurationRequest\",\n  \"description\": \"GetNotificationConfigurationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationId\": {\n      \"description\": \"The ID of the notification subscription configuration whose details are to be retrieved.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"notificationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-get-notification-configuration-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetNotificationConfigurationRequest
---
