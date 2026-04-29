---
description: CreateNotificationConfigurationRequest schema from Adyen API
layout: schema
name: CreateNotificationConfigurationRequest
properties_list:
- description: Details of the prospective notification subscription configuration.
  name: configurationDetails
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-configurations-create-notification-configuration-request-schema.json
slug: notification-configurations-create-notification-configuration-request
source_filename: notification-configurations-create-notification-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-create-notification-configuration-request-schema.json\",\n  \"title\": \"CreateNotificationConfigurationRequest\",\n  \"description\": \"CreateNotificationConfigurationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationDetails\": {\n      \"description\": \"Details of the prospective notification subscription configuration.\",\n      \"$ref\": \"#/components/schemas/NotificationConfigurationDetails\"\n    }\n  },\n  \"required\": [\n    \"configurationDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-configurations-create-notification-configuration-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateNotificationConfigurationRequest
---
