---
description: A Device Defender security profile behavior.
layout: schema
name: Behavior
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: metric
  type: object
- description: ''
  name: metricDimension
  type: object
- description: ''
  name: criteria
  type: object
- description: ''
  name: suppressAlerts
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-behavior-schema.json
slug: iot-core-behavior
source_filename: iot-core-behavior-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-behavior-schema.json\",\n  \"title\": \"Behavior\",\n  \"description\": \"A Device Defender security profile behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BehaviorName\"\n        },\n        {\n          \"description\": \"The name you've given to the behavior.\"\n        }\n      ]\n    },\n    \"metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BehaviorMetric\"\n        },\n        {\n          \"description\": \"What is measured by the behavior.\"\n        }\n      ]\n    },\n    \"metricDimension\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricDimension\"\n        },\n        {\n          \"description\": \"The dimension\
  \ for a metric in your behavior. For example, using a <code>TOPIC_FILTER</code> dimension, you can narrow down the scope of the metric to only MQTT topics where the name matches the pattern specified in the dimension. This can't be used with custom metrics.\"\n        }\n      ]\n    },\n    \"criteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BehaviorCriteria\"\n        },\n        {\n          \"description\": \"The criteria that determine if a device is behaving normally in regard to the <code>metric</code>.\"\n        }\n      ]\n    },\n    \"suppressAlerts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuppressAlerts\"\n        },\n        {\n          \"description\": \" Suppresses alerts. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-behavior-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: Behavior
---
