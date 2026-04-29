---
description: The configuration for notifications stored for each profiling group. This includes up to to two channels and a list of event publishers associated with each channel.
layout: schema
name: NotificationConfiguration
properties_list:
- description: ''
  name: channels
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-notification-configuration-schema.json
slug: amazon-codeguru-profiler-notification-configuration
source_filename: amazon-codeguru-profiler-notification-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-notification-configuration-schema.json\",\n  \"title\": \"NotificationConfiguration\",\n  \"description\": \"The configuration for notifications stored for each profiling group. This includes up to to two channels and a list of event publishers associated with each channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Channels\"\n        },\n        {\n          \"description\": \"List of up to two channels to be used for sending notifications for events detected from the application profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-notification-configuration-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: NotificationConfiguration
---
