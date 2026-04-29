---
description: 'The overrides that are sent to a container. An empty container override can be passed in. An example of an empty container override is <code>{"containerOverrides": [ ] }</code>. If a non-empty container override is specified, the <code>name</code> parameter must be included.'
layout: schema
name: EcsContainerOverride
properties_list:
- description: ''
  name: Command
  type: object
- description: ''
  name: Cpu
  type: object
- description: ''
  name: Environment
  type: object
- description: ''
  name: EnvironmentFiles
  type: object
- description: ''
  name: Memory
  type: object
- description: ''
  name: MemoryReservation
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ResourceRequirements
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-ecs-container-override-schema.json
slug: amazon-eventbridge-pipes-ecs-container-override
source_filename: amazon-eventbridge-pipes-ecs-container-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-container-override-schema.json\",\n  \"title\": \"EcsContainerOverride\",\n  \"description\": \"The overrides that are sent to a container. An empty container override can be passed in. An example of an empty container override is <code>{\\\"containerOverrides\\\": [ ] }</code>. If a non-empty container override is specified, the <code>name</code> parameter must be included.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The command to send to the container that overrides the default command from the Docker image or the task definition. You must also specify a container name.\"\n        }\n      ]\n    },\n\
  \    \"Cpu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of <code>cpu</code> units reserved for the container, instead of the default value from the task definition. You must also specify a container name.\"\n        }\n      ]\n    },\n    \"Environment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsEnvironmentVariableList\"\n        },\n        {\n          \"description\": \"The environment variables to send to the container. You can add new environment variables, which are added to the container at launch, or you can override the existing environment variables from the Docker image or the task definition. You must also specify a container name.\"\n        }\n      ]\n    },\n    \"EnvironmentFiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsEnvironmentFileList\"\n        },\n        {\n          \"description\"\
  : \"A list of files containing the environment variables to pass to a container, instead of the value from the container definition.\"\n        }\n      ]\n    },\n    \"Memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The hard limit (in MiB) of memory to present to the container, instead of the default value from the task definition. If your container attempts to exceed the memory specified here, the container is killed. You must also specify a container name.\"\n        }\n      ]\n    },\n    \"MemoryReservation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The soft limit (in MiB) of memory to reserve for the container, instead of the default value from the task definition. You must also specify a container name.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the container that receives the override. This parameter is required if any override is specified.\"\n        }\n      ]\n    },\n    \"ResourceRequirements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsResourceRequirementsList\"\n        },\n        {\n          \"description\": \"The type and amount of a resource to assign to a container, instead of the default value from the task definition. The only supported resource is a GPU.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-container-override-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: EcsContainerOverride
---
