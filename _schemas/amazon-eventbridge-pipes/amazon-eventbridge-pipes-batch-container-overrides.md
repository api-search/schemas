---
description: The overrides that are sent to a container.
layout: schema
name: BatchContainerOverrides
properties_list:
- description: ''
  name: Command
  type: object
- description: ''
  name: Environment
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: ResourceRequirements
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-batch-container-overrides-schema.json
slug: amazon-eventbridge-pipes-batch-container-overrides
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-container-overrides-schema.json\",\n  \"title\": \"BatchContainerOverrides\",\n  \"description\": \"The overrides that are sent to a container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The command to send to the container that overrides the default command from the Docker image or the task definition.\"\n        }\n      ]\n    },\n    \"Environment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchEnvironmentVariableList\"\n        },\n        {\n          \"description\": \"<p>The environment variables to send to the container. You can add new environment variables,\
  \ which are added to the container at launch, or you can override the existing environment variables from the Docker image or the task definition.</p> <note> <p>Environment variables cannot start with \\\"<code>Batch</code>\\\". This naming convention is reserved for variables that Batch sets.</p> </note>\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The instance type to use for a multi-node parallel job.</p> <note> <p>This parameter isn't applicable to single-node container jobs or jobs that run on Fargate resources, and shouldn't be provided.</p> </note>\"\n        }\n      ]\n    },\n    \"ResourceRequirements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchResourceRequirementsList\"\n        },\n        {\n          \"description\": \"The type and amount of resources to assign to a container. This overrides\
  \ the settings in the job definition. The supported resources include <code>GPU</code>, <code>MEMORY</code>, and <code>VCPU</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-container-overrides-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: BatchContainerOverrides
---
