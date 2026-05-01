---
description: The type and amount of a resource to assign to a container. The supported resource types are GPUs and Elastic Inference accelerators. For more information, see <a href="https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html">Working with GPUs on Amazon ECS</a> or <a href="https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-inference.html">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>
layout: schema
name: EcsResourceRequirement
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-ecs-resource-requirement-schema.json
slug: amazon-eventbridge-pipes-ecs-resource-requirement
source_filename: amazon-eventbridge-pipes-ecs-resource-requirement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-resource-requirement-schema.json\",\n  \"title\": \"EcsResourceRequirement\",\n  \"description\": \"The type and amount of a resource to assign to a container. The supported resource types are GPUs and Elastic Inference accelerators. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html\\\">Working with GPUs on Amazon ECS</a> or <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-inference.html\\\">Working with Amazon Elastic Inference on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i> \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsResourceRequirementType\"\n\
  \        },\n        {\n          \"description\": \"The type of resource to assign to a container. The supported values are <code>GPU</code> or <code>InferenceAccelerator</code>.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The value for the specified resource type.</p> <p>If the <code>GPU</code> type is used, the value is the number of physical <code>GPUs</code> the Amazon ECS container agent reserves for the container. The number of GPUs that's reserved for all containers in a task can't exceed the number of available GPUs on the container instance that the task is launched on.</p> <p>If the <code>InferenceAccelerator</code> type is used, the <code>value</code> matches the <code>deviceName</code> for an InferenceAccelerator specified in a task definition.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"value\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-resource-requirement-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: EcsResourceRequirement
---
