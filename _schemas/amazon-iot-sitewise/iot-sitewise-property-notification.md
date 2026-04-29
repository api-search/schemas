---
description: Contains asset property value notification information. When the notification state is enabled, IoT SiteWise publishes property value updates to a unique MQTT topic. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/userguide/interact-with-other-services.html">Interacting with other services</a> in the <i>IoT SiteWise User Guide</i>.
layout: schema
name: PropertyNotification
properties_list:
- description: ''
  name: topic
  type: object
- description: ''
  name: state
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-property-notification-schema.json
slug: iot-sitewise-property-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-property-notification-schema.json\",\n  \"title\": \"PropertyNotification\",\n  \"description\": \"Contains asset property value notification information. When the notification state is enabled, IoT SiteWise publishes property value updates to a unique MQTT topic. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/interact-with-other-services.html\\\">Interacting with other services</a> in the <i>IoT SiteWise User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyNotificationTopic\"\n        },\n        {\n          \"description\": \"The MQTT topic to which IoT SiteWise publishes property value update notifications.\"\n        }\n\
  \      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyNotificationState\"\n        },\n        {\n          \"description\": \"The current notification state.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"topic\",\n    \"state\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-property-notification-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: PropertyNotification
---
