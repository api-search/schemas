---
description: Contains information about an event source for an Lambda function. The event source defines the topics on which this Lambda function subscribes to receive messages that run the function.
layout: schema
name: LambdaEventSource
properties_list:
- description: ''
  name: topic
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-event-source-schema.json
slug: iot-greengrass-lambda-event-source
source_filename: iot-greengrass-lambda-event-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-event-source-schema.json\",\n  \"title\": \"LambdaEventSource\",\n  \"description\": \"Contains information about an event source for an Lambda function. The event source defines the topics on which this Lambda function subscribes to receive messages that run the function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TopicString\"\n        },\n        {\n          \"description\": \"The topic to which to subscribe to receive event messages.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaEventSourceType\"\n        },\n        {\n          \"description\": \"<p>The type of event source. Choose from the\
  \ following options:</p> <ul> <li> <p> <code>PUB_SUB</code> \\u2013 Subscribe to local publish/subscribe messages. This event source type doesn't support MQTT wildcards (<code>+</code> and <code>#</code>) in the event source topic.</p> </li> <li> <p> <code>IOT_CORE</code> \\u2013 Subscribe to Amazon Web Services IoT Core MQTT messages. This event source type supports MQTT wildcards (<code>+</code> and <code>#</code>) in the event source topic.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"topic\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-event-source-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaEventSource
---
