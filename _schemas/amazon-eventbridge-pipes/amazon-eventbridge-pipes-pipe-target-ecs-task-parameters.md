---
description: The parameters for using an Amazon ECS task as a target.
layout: schema
name: PipeTargetEcsTaskParameters
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
  name: Overrides
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
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-ecs-task-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-ecs-task-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-ecs-task-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-ecs-task-parameters-schema.json\",\n  \"title\": \"PipeTargetEcsTaskParameters\",\n  \"description\": \"The parameters for using an Amazon ECS task as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CapacityProviderStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityProviderStrategy\"\n        },\n        {\n          \"description\": \"<p>The capacity provider strategy to use for the task.</p> <p>If a <code>capacityProviderStrategy</code> is specified, the <code>launchType</code> parameter must be omitted. If no <code>capacityProviderStrategy</code> or launchType is specified, the <code>defaultCapacityProviderStrategy</code> for the cluster is used. </p>\"\n        }\n      ]\n    },\n    \"EnableECSManagedTags\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable Amazon ECS managed tags for the task. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html\\\">Tagging Your Amazon ECS Resources</a> in the Amazon Elastic Container Service Developer Guide. \"\n        }\n      ]\n    },\n    \"EnableExecuteCommand\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether or not to enable the execute command functionality for the containers in this task. If true, this enables execute command functionality on all containers in the task.\"\n        }\n      ]\n    },\n    \"Group\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specifies an\
  \ Amazon ECS task group for the task. The maximum length is 255 characters.\"\n        }\n      ]\n    },\n    \"LaunchType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchType\"\n        },\n        {\n          \"description\": \"Specifies the launch type on which your task is running. The launch type that you specify here must match one of the launch type (compatibilities) of the target task. The <code>FARGATE</code> value is supported only in the Regions where Fargate with Amazon ECS is supported. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/AWS-Fargate.html\\\">Fargate on Amazon ECS</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"NetworkConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkConfiguration\"\n        },\n        {\n          \"description\": \"<p>Use this structure if the Amazon\
  \ ECS task uses the <code>awsvpc</code> network mode. This structure specifies the VPC subnets and security groups associated with the task, and whether a public IP address is to be used. This structure is required if <code>LaunchType</code> is <code>FARGATE</code> because the <code>awsvpc</code> mode is required for Fargate tasks.</p> <p>If you specify <code>NetworkConfiguration</code> when the target ECS task does not use the <code>awsvpc</code> network mode, the task fails.</p>\"\n        }\n      ]\n    },\n    \"Overrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsTaskOverride\"\n        },\n        {\n          \"description\": \"The overrides that are associated with a task.\"\n        }\n      ]\n    },\n    \"PlacementConstraints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementConstraints\"\n        },\n        {\n          \"description\": \"An array of placement constraint objects to use for the\
  \ task. You can specify up to 10 constraints per task (including constraints in the task definition and those specified at runtime).\"\n        }\n      ]\n    },\n    \"PlacementStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlacementStrategies\"\n        },\n        {\n          \"description\": \"The placement strategy objects to use for the task. You can specify a maximum of five strategy rules per task. \"\n        }\n      ]\n    },\n    \"PlatformVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Specifies the platform version for the task. Specify only the numeric portion of the platform version, such as <code>1.1.0</code>.</p> <p>This structure is used only if <code>LaunchType</code> is <code>FARGATE</code>. For more information about valid platform versions, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/developerguide/platform_versions.html\\\
  \">Fargate Platform Versions</a> in the <i>Amazon Elastic Container Service Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"PropagateTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropagateTags\"\n        },\n        {\n          \"description\": \"Specifies whether to propagate the tags from the task definition to the task. If no value is specified, the tags are not propagated. Tags can only be propagated to the task during task creation. To add tags to a task after task creation, use the <code>TagResource</code> API action. \"\n        }\n      ]\n    },\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceId\"\n        },\n        {\n          \"description\": \"The reference ID to use for the task.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\"\
  : \"The metadata that you apply to the task to help you categorize and organize them. Each tag consists of a key and an optional value, both of which you define. To learn more, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_RunTask.html#ECS-RunTask-request-tags\\\">RunTask</a> in the Amazon ECS API Reference.\"\n        }\n      ]\n    },\n    \"TaskCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMin1\"\n        },\n        {\n          \"description\": \"The number of tasks to create based on <code>TaskDefinition</code>. The default is 1.\"\n        }\n      ]\n    },\n    \"TaskDefinitionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnOrJsonPath\"\n        },\n        {\n          \"description\": \"The ARN of the task definition to use if the event target is an Amazon ECS task. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TaskDefinitionArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-ecs-task-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetEcsTaskParameters
---
