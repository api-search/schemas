---
description: Parameters to define a mitigation action that publishes findings to Amazon SNS. You can implement your own custom actions in response to the Amazon SNS messages.
layout: schema
name: PublishFindingToSnsParams
properties_list:
- description: ''
  name: topicArn
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-publish-finding-to-sns-params-schema.json
slug: iot-device-defender-publish-finding-to-sns-params
source_filename: iot-device-defender-publish-finding-to-sns-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-publish-finding-to-sns-params-schema.json\",\n  \"title\": \"PublishFindingToSnsParams\",\n  \"description\": \"Parameters to define a mitigation action that publishes findings to Amazon SNS. You can implement your own custom actions in response to the Amazon SNS messages.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopicArn\"\n        },\n        {\n          \"description\": \"The ARN of the topic to which you want to publish the findings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"topicArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-publish-finding-to-sns-params-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: PublishFindingToSnsParams
---
