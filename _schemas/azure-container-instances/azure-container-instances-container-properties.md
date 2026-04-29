---
description: The container instance properties.
layout: schema
name: ContainerProperties
properties_list:
- description: The commands to execute within the container instance in exec form.
  name: command
  type: array
- description: The environment variables to set in the container instance.
  name: environmentVariables
  type: array
- description: The name of the image used to create the container instance.
  name: image
  type: string
- description: The instance view of the container instance. Only valid in response.
  name: instanceView
  type: object
- description: The liveness probe.
  name: livenessProbe
  type: object
- description: The exposed ports on the container instance.
  name: ports
  type: array
- description: The readiness probe.
  name: readinessProbe
  type: object
- description: The resource requirements of the container instance.
  name: resources
  type: object
- description: The volume mounts available to the container instance.
  name: volumeMounts
  type: array
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-properties-schema.json
slug: azure-container-instances-container-properties
source_filename: azure-container-instances-container-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-properties-schema.json\",\n  \"title\": \"ContainerProperties\",\n  \"description\": \"The container instance properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"command\": {\n      \"description\": \"The commands to execute within the container instance in exec form.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"environmentVariables\": {\n      \"description\": \"The environment variables to set in the container instance.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/EnvironmentVariable\"\n      },\n      \"type\": \"array\"\n    },\n    \"image\": {\n      \"description\": \"The name of the image used to create the container instance.\",\n      \"type\": \"string\"\n  \
  \  },\n    \"instanceView\": {\n      \"description\": \"The instance view of the container instance. Only valid in response.\",\n      \"properties\": {\n        \"currentState\": {\n          \"$ref\": \"#/definitions/ContainerState\",\n          \"description\": \"Current container instance state.\",\n          \"readOnly\": true\n        },\n        \"events\": {\n          \"description\": \"The events of the container instance.\",\n          \"items\": {\n            \"$ref\": \"#/definitions/Event\"\n          },\n          \"readOnly\": true,\n          \"type\": \"array\"\n        },\n        \"previousState\": {\n          \"$ref\": \"#/definitions/ContainerState\",\n          \"description\": \"Previous container instance state.\",\n          \"readOnly\": true\n        },\n        \"restartCount\": {\n          \"description\": \"The number of times that the container instance has been restarted.\",\n          \"readOnly\": true,\n          \"type\": \"integer\"\n        }\n\
  \      },\n      \"readOnly\": true,\n      \"type\": \"object\"\n    },\n    \"livenessProbe\": {\n      \"$ref\": \"#/definitions/ContainerProbe\",\n      \"description\": \"The liveness probe.\"\n    },\n    \"ports\": {\n      \"description\": \"The exposed ports on the container instance.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ContainerPort\"\n      },\n      \"type\": \"array\"\n    },\n    \"readinessProbe\": {\n      \"$ref\": \"#/definitions/ContainerProbe\",\n      \"description\": \"The readiness probe.\"\n    },\n    \"resources\": {\n      \"$ref\": \"#/definitions/ResourceRequirements\",\n      \"description\": \"The resource requirements of the container instance.\"\n    },\n    \"volumeMounts\": {\n      \"description\": \"The volume mounts available to the container instance.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/VolumeMount\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"resources\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-container-properties-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerProperties
---
