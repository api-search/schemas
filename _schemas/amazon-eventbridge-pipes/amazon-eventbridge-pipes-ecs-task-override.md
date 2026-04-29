---
description: The overrides that are associated with a task.
layout: schema
name: EcsTaskOverride
properties_list:
- description: ''
  name: ContainerOverrides
  type: object
- description: ''
  name: Cpu
  type: object
- description: ''
  name: EphemeralStorage
  type: object
- description: ''
  name: ExecutionRoleArn
  type: object
- description: ''
  name: InferenceAcceleratorOverrides
  type: object
- description: ''
  name: Memory
  type: object
- description: ''
  name: TaskRoleArn
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-ecs-task-override-schema.json
slug: amazon-eventbridge-pipes-ecs-task-override
source_filename: amazon-eventbridge-pipes-ecs-task-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-task-override-schema.json\",\n  \"title\": \"EcsTaskOverride\",\n  \"description\": \"The overrides that are associated with a task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerOverrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsContainerOverrideList\"\n        },\n        {\n          \"description\": \"One or more container overrides that are sent to a task.\"\n        }\n      ]\n    },\n    \"Cpu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The cpu override for the task.\"\n        }\n      ]\n    },\n    \"EphemeralStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsEphemeralStorage\"\
  \n        },\n        {\n          \"description\": \"<p>The ephemeral storage setting override for the task.</p> <note> <p>This parameter is only supported for tasks hosted on Fargate that use the following platform versions:</p> <ul> <li> <p>Linux platform version <code>1.4.0</code> or later.</p> </li> <li> <p>Windows platform version <code>1.0.0</code> or later.</p> </li> </ul> </note>\"\n        }\n      ]\n    },\n    \"ExecutionRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnOrJsonPath\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the task execution IAM role override for the task. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_execution_IAM_role.html\\\">Amazon ECS task execution IAM role</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"InferenceAcceleratorOverrides\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/EcsInferenceAcceleratorOverrideList\"\n        },\n        {\n          \"description\": \"The Elastic Inference accelerator override for the task.\"\n        }\n      ]\n    },\n    \"Memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The memory override for the task.\"\n        }\n      ]\n    },\n    \"TaskRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnOrJsonPath\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that containers in this task can assume. All containers in this task are granted the permissions that are specified in this role. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task-iam-roles.html\\\">IAM Role for Tasks</a> in the <i>Amazon Elastic Container Service Developer\
  \ Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-task-override-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: EcsTaskOverride
---
