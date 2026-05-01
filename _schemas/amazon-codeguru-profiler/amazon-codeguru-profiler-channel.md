---
description: Notification medium for users to get alerted for events that occur in application profile. We support SNS topic as a notification channel.
layout: schema
name: Channel
properties_list:
- description: ''
  name: eventPublishers
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: uri
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-channel-schema.json
slug: amazon-codeguru-profiler-channel
source_filename: amazon-codeguru-profiler-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-channel-schema.json\",\n  \"title\": \"Channel\",\n  \"description\": \"Notification medium for users to get alerted for events that occur in application profile. We support SNS topic as a notification channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventPublishers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventPublishers\"\n        },\n        {\n          \"description\": \"List of publishers for different type of events that may be detected in an application from the profile. Anomaly detection is the only event publisher in Profiler.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelId\"\n        },\n        {\n          \"description\"\
  : \"Unique identifier for each <code>Channel</code> in the notification configuration of a Profiling Group. A random UUID for channelId is used when adding a channel to the notification configuration if not specified in the request.\"\n        }\n      ]\n    },\n    \"uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelUri\"\n        },\n        {\n          \"description\": \"Unique arn of the resource to be used for notifications. We support a valid SNS topic arn as a channel uri.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventPublishers\",\n    \"uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-channel-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: Channel
---
