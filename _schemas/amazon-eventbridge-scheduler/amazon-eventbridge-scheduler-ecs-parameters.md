---
description: The templated target type for the Amazon ECS <a href="https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_RunTask.html"> <code>RunTask</code> </a> API operation.
layout: schema
name: EcsParameters
properties_list:
- description: ''
  name: CapacityProviderStrategy
  type: object
- description: ''
  name: EnableECSManagedTags
  type: object
- description: ''
  name: EnableExecuteCommand
  type: object
- description: ''
  name: Group
  type: object
- description: ''
  name: LaunchType
  type: object
- description: ''
  name: NetworkConfiguration
  type: object
- description: ''
  name: PlacementConstraints
  type: object
- description: ''
  name: PlacementStrategy
  type: object
- description: ''
  name: PlatformVersion
  type: object
- description: ''
  name: PropagateTags
  type: object
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: TaskCount
  type: object
- description: ''
  name: TaskDefinitionArn
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-ecs-parameters-schema.json
slug: amazon-eventbridge-scheduler-ecs-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-ecs-parameters-schema.json\",\n  \"title\": \"EcsParameters\",\n  \"description\": \"The templated target type for the Amazon ECS <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_RunTask.html\\\"> <code>RunTask</code> </a> API operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CapacityProviderStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityProviderStrategy\"\n        },\n        {\n          \"description\": \"The capacity provider strategy to use for the task.\"\n        }\n      ]\n    },\n    \"EnableECSManagedTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnableECSManagedTags\"\n        },\n        {\n          \"description\": \"\
  Specifies whether to enable Amazon ECS managed tags for the task. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html\\\">Tagging Your Amazon ECS Resources</a> in the <i>Amazon ECS Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"EnableExecuteCommand\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnableExecuteCommand\"\n        },\n        {\n          \"description\": \"Whether or not to enable the execute command functionality for the containers in this task. If true, this enables execute command functionality on all containers in the task.\"\n        }\n      ]\n    },\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Group\"\n        },\n        {\n          \"description\": \"Specifies an ECS task group for the task. The maximum length is 255 characters.\"\n        }\n      ]\n    },\n    \"LaunchType\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/LaunchType\"\n        },\n        {\n          \"description\": \"Specifies the launch type on which your task is running. The launch type that you specify here must match one of the launch type (compatibilities) of the target task. The <code>FARGATE</code> value is supported only in the Regions where Fargate with Amazon ECS is supported. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS_Fargate.html\\\">AWS Fargate on Amazon ECS</a> in the <i>Amazon ECS Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"NetworkConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkConfiguration\"\n        },\n        {\n          \"description\": \"This structure specifies the network configuration for an ECS task.\"\n        }\n      ]\n    },\n    \"PlacementConstraints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementConstraints\"\
  \n        },\n        {\n          \"description\": \"An array of placement constraint objects to use for the task. You can specify up to 10 constraints per task (including constraints in the task definition and those specified at runtime).\"\n        }\n      ]\n    },\n    \"PlacementStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementStrategies\"\n        },\n        {\n          \"description\": \"The task placement strategy for a task or service.\"\n        }\n      ]\n    },\n    \"PlatformVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlatformVersion\"\n        },\n        {\n          \"description\": \"Specifies the platform version for the task. Specify only the numeric portion of the platform version, such as <code>1.1.0</code>.\"\n        }\n      ]\n    },\n    \"PropagateTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropagateTags\"\n        },\n  \
  \      {\n          \"description\": \"Specifies whether to propagate the tags from the task definition to the task. If no value is specified, the tags are not propagated. Tags can only be propagated to the task during task creation. To add tags to a task after task creation, use Amazon ECS's <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TagResource.html\\\"> <code>TagResource</code> </a> API action. \"\n        }\n      ]\n    },\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceId\"\n        },\n        {\n          \"description\": \"The reference ID to use for the task.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The metadata that you apply to the task to help you categorize and organize them. Each tag consists of a key and an optional value, both of which you define.\
  \ For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_RunTask.html\\\"> <code>RunTask</code> </a> in the <i>Amazon ECS API Reference</i>.\"\n        }\n      ]\n    },\n    \"TaskCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskCount\"\n        },\n        {\n          \"description\": \"The number of tasks to create based on <code>TaskDefinition</code>. The default is <code>1</code>.\"\n        }\n      ]\n    },\n    \"TaskDefinitionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskDefinitionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the task definition to use if the event target is an Amazon ECS task.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TaskDefinitionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-ecs-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: EcsParameters
---
