---
description: The structure representing the GetNotificationConfigurationResponse.
layout: schema
name: GetNotificationConfigurationResponse
properties_list:
- description: ''
  name: notificationConfiguration
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-get-notification-configuration-response-schema.json
slug: amazon-codeguru-profiler-get-notification-configuration-response
source_filename: amazon-codeguru-profiler-get-notification-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-notification-configuration-response-schema.json\",\n  \"title\": \"GetNotificationConfigurationResponse\",\n  \"description\": \"The structure representing the GetNotificationConfigurationResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationConfiguration\"\n        },\n        {\n          \"description\": \"The current notification configuration for this profiling group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"notificationConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-notification-configuration-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: GetNotificationConfigurationResponse
---
