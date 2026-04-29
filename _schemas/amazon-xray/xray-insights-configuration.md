---
description: The structure containing configurations related to insights.
layout: schema
name: InsightsConfiguration
properties_list:
- description: ''
  name: InsightsEnabled
  type: object
- description: ''
  name: NotificationsEnabled
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-insights-configuration-schema.json
slug: xray-insights-configuration
source_filename: xray-insights-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsightsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Set the InsightsEnabled value to true to enable insights or false to disable insights.\"\n        }\n      ]\n    },\n    \"NotificationsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Set the NotificationsEnabled value to true to enable insights notifications. Notifications can only be enabled on a group with InsightsEnabled set to true.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The structure containing configurations related to insights.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsightsConfiguration\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insights-configuration-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insights-configuration-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: InsightsConfiguration
---
