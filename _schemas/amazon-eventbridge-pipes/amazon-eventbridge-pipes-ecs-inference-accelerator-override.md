---
description: Details on an Elastic Inference accelerator task override. This parameter is used to override the Elastic Inference accelerator specified in the task definition. For more information, see <a href="https://docs.aws.amazon.com/AmazonECS/latest/userguide/ecs-inference.html">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.
layout: schema
name: EcsInferenceAcceleratorOverride
properties_list:
- description: ''
  name: deviceName
  type: object
- description: ''
  name: deviceType
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-ecs-inference-accelerator-override-schema.json
slug: amazon-eventbridge-pipes-ecs-inference-accelerator-override
source_filename: amazon-eventbridge-pipes-ecs-inference-accelerator-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-inference-accelerator-override-schema.json\",\n  \"title\": \"EcsInferenceAcceleratorOverride\",\n  \"description\": \"Details on an Elastic Inference accelerator task override. This parameter is used to override the Elastic Inference accelerator specified in the task definition. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/ecs-inference.html\\\">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Elastic Inference accelerator device name to\
  \ override for the task. This parameter must match a <code>deviceName</code> specified in the task definition.\"\n        }\n      ]\n    },\n    \"deviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Elastic Inference accelerator type to use.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-inference-accelerator-override-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: EcsInferenceAcceleratorOverride
---
