---
description: The structure representing the AddNotificationChannelsRequest.
layout: schema
name: AddNotificationChannelsRequest
properties_list:
- description: ''
  name: channels
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-add-notification-channels-request-schema.json
slug: amazon-codeguru-profiler-add-notification-channels-request
source_filename: amazon-codeguru-profiler-add-notification-channels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-add-notification-channels-request-schema.json\",\n  \"title\": \"AddNotificationChannelsRequest\",\n  \"description\": \"The structure representing the AddNotificationChannelsRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Channels\"\n        },\n        {\n          \"description\": \"One or 2 channels to report to when anomalies are detected.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channels\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-add-notification-channels-request-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: AddNotificationChannelsRequest
---
