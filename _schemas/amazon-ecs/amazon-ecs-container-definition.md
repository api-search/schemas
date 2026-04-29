---
description: A container definition describes a container within a task definition.
layout: schema
name: ContainerDefinition
properties_list:
- description: The name of a container. Up to 255 characters (uppercase and lowercase letters, numbers, underscores, and hyphens).
  name: name
  type: string
- description: The image used to start a container. Images in the Docker Hub registry are available by default. You can also specify an ECR repository.
  name: image
  type: string
- description: The number of cpu units reserved for the container.
  name: cpu
  type: integer
- description: The amount (in MiB) of memory to present to the container. Corresponds to the hard limit.
  name: memory
  type: integer
- description: The soft limit (in MiB) of memory to reserve for the container.
  name: memoryReservation
  type: integer
- description: Allows containers to communicate without port mappings. Only supported for bridge network mode.
  name: links
  type: array
- description: The list of port mappings for the container.
  name: portMappings
  type: array
- description: If the essential parameter of a container is marked as true and that container fails or stops, all other containers that are part of the task are stopped.
  name: essential
  type: boolean
- description: The entry point that is passed to the container.
  name: entryPoint
  type: array
- description: The command that is passed to the container.
  name: command
  type: array
- description: The environment variables to pass to a container.
  name: environment
  type: array
- description: A list of files containing the environment variables to pass to a container.
  name: environmentFiles
  type: array
- description: The mount points for data volumes in your container.
  name: mountPoints
  type: array
- description: Data volumes to mount from another container.
  name: volumesFrom
  type: array
- description: The secrets to pass to the container from AWS Secrets Manager or SSM Parameter Store.
  name: secrets
  type: array
- description: The dependencies defined for container startup and shutdown.
  name: dependsOn
  type: array
- description: Time duration (in seconds) to wait before giving up on resolving dependencies for a container.
  name: startTimeout
  type: integer
- description: Time duration (in seconds) to wait before the container is forcefully killed if it does not exit normally on its own.
  name: stopTimeout
  type: integer
- description: ''
  name: hostname
  type: string
- description: The user to run as inside the container.
  name: user
  type: string
- description: The working directory to run commands inside the container in.
  name: workingDirectory
  type: string
- description: ''
  name: disableNetworking
  type: boolean
- description: When this parameter is true, the container is given elevated privileges on the host container instance.
  name: privileged
  type: boolean
- description: When this parameter is true, the container is given read-only access to its root file system.
  name: readonlyRootFilesystem
  type: boolean
- description: ''
  name: dnsServers
  type: array
- description: ''
  name: dnsSearchDomains
  type: array
- description: ''
  name: extraHosts
  type: array
- description: ''
  name: dockerSecurityOptions
  type: array
- description: ''
  name: interactive
  type: boolean
- description: ''
  name: pseudoTerminal
  type: boolean
- description: A key/value map of labels to add to the container.
  name: dockerLabels
  type: object
- description: ''
  name: ulimits
  type: array
- description: ''
  name: systemControls
  type: array
- description: ''
  name: resourceRequirements
  type: array
- description: ''
  name: firelensConfiguration
  type: object
- description: ''
  name: repositoryCredentials
  type: object
- description: ''
  name: restartPolicy
  type: object
- description: ''
  name: credentialSpecs
  type: array
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-container-definition-schema.json
slug: amazon-ecs-container-definition
source_filename: amazon-ecs-container-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerDefinition\",\n  \"type\": \"object\",\n  \"description\": \"A container definition describes a container within a task definition.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a container. Up to 255 characters (uppercase and lowercase letters, numbers, underscores, and hyphens).\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"The image used to start a container. Images in the Docker Hub registry are available by default. You can also specify an ECR repository.\"\n    },\n    \"cpu\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of cpu units reserved for the container.\"\n    },\n    \"memory\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount (in MiB) of memory to present to the container. Corresponds to the hard limit.\"\n    },\n    \"memoryReservation\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The soft limit (in MiB) of memory to reserve for the container.\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"Allows containers to communicate without port mappings. Only supported for bridge network mode.\"\n    },\n    \"portMappings\": {\n      \"type\": \"array\",\n      \"description\": \"The list of port mappings for the container.\"\n    },\n    \"essential\": {\n      \"type\": \"boolean\",\n      \"description\": \"If the essential parameter of a container is marked as true and that container fails or stops, all other containers that are part of the task are stopped.\"\n    },\n    \"entryPoint\": {\n      \"type\": \"array\",\n      \"description\": \"The entry point that is passed to the container.\"\n    },\n    \"command\": {\n      \"type\": \"array\",\n      \"description\": \"The command that is passed to the container.\"\n    },\n    \"environment\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"The environment variables to pass to a container.\"\n    },\n    \"environmentFiles\": {\n      \"type\": \"array\",\n      \"description\": \"A list of files containing the environment variables to pass to a container.\"\n    },\n    \"mountPoints\": {\n      \"type\": \"array\",\n      \"description\": \"The mount points for data volumes in your container.\"\n    },\n    \"volumesFrom\": {\n      \"type\": \"array\",\n      \"description\": \"Data volumes to mount from another container.\"\n    },\n    \"secrets\": {\n      \"type\": \"array\",\n      \"description\": \"The secrets to pass to the container from AWS Secrets Manager or SSM Parameter Store.\"\n    },\n    \"dependsOn\": {\n      \"type\": \"array\",\n      \"description\": \"The dependencies defined for container startup and shutdown.\"\n    },\n    \"startTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Time duration (in seconds) to wait before giving up on resolving dependencies\
  \ for a container.\"\n    },\n    \"stopTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Time duration (in seconds) to wait before the container is forcefully killed if it does not exit normally on its own.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The user to run as inside the container.\"\n    },\n    \"workingDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"The working directory to run commands inside the container in.\"\n    },\n    \"disableNetworking\": {\n      \"type\": \"boolean\"\n    },\n    \"privileged\": {\n      \"type\": \"boolean\",\n      \"description\": \"When this parameter is true, the container is given elevated privileges on the host container instance.\"\n    },\n    \"readonlyRootFilesystem\": {\n      \"type\": \"boolean\",\n      \"description\": \"When this parameter is true, the container is given read-only access to its\
  \ root file system.\"\n    },\n    \"dnsServers\": {\n      \"type\": \"array\"\n    },\n    \"dnsSearchDomains\": {\n      \"type\": \"array\"\n    },\n    \"extraHosts\": {\n      \"type\": \"array\"\n    },\n    \"dockerSecurityOptions\": {\n      \"type\": \"array\"\n    },\n    \"interactive\": {\n      \"type\": \"boolean\"\n    },\n    \"pseudoTerminal\": {\n      \"type\": \"boolean\"\n    },\n    \"dockerLabels\": {\n      \"type\": \"object\",\n      \"description\": \"A key/value map of labels to add to the container.\"\n    },\n    \"ulimits\": {\n      \"type\": \"array\"\n    },\n    \"systemControls\": {\n      \"type\": \"array\"\n    },\n    \"resourceRequirements\": {\n      \"type\": \"array\"\n    },\n    \"firelensConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"repositoryCredentials\": {\n      \"type\": \"object\"\n    },\n    \"restartPolicy\": {\n      \"type\": \"object\"\n    },\n    \"credentialSpecs\": {\n      \"type\": \"array\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-container-definition-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ContainerDefinition
---
