---
description: Schema defining the structure of an AWS App Runner service resource, including source configuration, instance configuration, networking, auto scaling, health checks, and observability settings.
layout: schema
name: AWS App Runner Service
properties_list:
- description: The customer-provided service name.
  name: ServiceName
  type: string
- description: An ID that App Runner generated for this service.
  name: ServiceId
  type: string
- description: The Amazon Resource Name (ARN) of the service.
  name: ServiceArn
  type: string
- description: A subdomain URL for the App Runner service.
  name: ServiceUrl
  type: string
- description: The current state of the App Runner service.
  name: Status
  type: string
- description: ''
  name: SourceConfiguration
  type: object
- description: ''
  name: InstanceConfiguration
  type: object
- description: ''
  name: AutoScalingConfigurationSummary
  type: object
- description: ''
  name: HealthCheckConfiguration
  type: object
- description: ''
  name: NetworkConfiguration
  type: object
- description: ''
  name: ObservabilityConfiguration
  type: object
- description: The time when the service was created.
  name: CreatedAt
  type: string
- description: The time when the service was last updated.
  name: UpdatedAt
  type: string
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-schema.json
slug: amazon-app-runner
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-app-runner/service\",\n  \"title\": \"AWS App Runner Service\",\n  \"description\": \"Schema defining the structure of an AWS App Runner service resource, including source configuration, instance configuration, networking, auto scaling, health checks, and observability settings.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ServiceName\",\n    \"SourceConfiguration\"\n  ],\n  \"properties\": {\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"The customer-provided service name.\",\n      \"pattern\": \"^[A-Za-z0-9][A-Za-z0-9-_]{3,39}$\"\n    },\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"An ID that App Runner generated for this service.\"\n    },\n    \"ServiceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the service.\"\n    },\n   \
  \ \"ServiceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A subdomain URL for the App Runner service.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_FAILED\",\n        \"RUNNING\",\n        \"DELETED\",\n        \"DELETE_FAILED\",\n        \"PAUSED\",\n        \"OPERATION_IN_PROGRESS\"\n      ],\n      \"description\": \"The current state of the App Runner service.\"\n    },\n    \"SourceConfiguration\": {\n      \"$ref\": \"#/$defs/SourceConfiguration\"\n    },\n    \"InstanceConfiguration\": {\n      \"$ref\": \"#/$defs/InstanceConfiguration\"\n    },\n    \"AutoScalingConfigurationSummary\": {\n      \"$ref\": \"#/$defs/AutoScalingConfigurationSummary\"\n    },\n    \"HealthCheckConfiguration\": {\n      \"$ref\": \"#/$defs/HealthCheckConfiguration\"\n    },\n    \"NetworkConfiguration\": {\n      \"$ref\": \"#/$defs/NetworkConfiguration\"\n    },\n    \"ObservabilityConfiguration\": {\n      \"$ref\": \"#/$defs/ServiceObservabilityConfiguration\"\
  \n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the service was created.\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the service was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"SourceConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the source deployed to the App Runner service.\",\n      \"properties\": {\n        \"CodeRepository\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"RepositoryUrl\": {\n              \"type\": \"string\"\n            },\n            \"SourceCodeVersion\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"BRANCH\"\n                  ]\n                },\n          \
  \      \"Value\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"CodeConfiguration\": {\n              \"type\": \"object\"\n            }\n          }\n        },\n        \"ImageRepository\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ImageIdentifier\": {\n              \"type\": \"string\"\n            },\n            \"ImageRepositoryType\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"ECR\",\n                \"ECR_PUBLIC\"\n              ]\n            },\n            \"ImageConfiguration\": {\n              \"type\": \"object\"\n            }\n          }\n        },\n        \"AutoDeploymentsEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether continuous integration from the source repository is enabled.\"\n        },\n        \"AuthenticationConfiguration\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"ConnectionArn\": {\n              \"type\": \"string\"\n            },\n            \"AccessRoleArn\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"InstanceConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the runtime configuration of an App Runner service instance.\",\n      \"properties\": {\n        \"Cpu\": {\n          \"type\": \"string\",\n          \"description\": \"The number of CPU units reserved for each instance.\",\n          \"enum\": [\n            \"256\",\n            \"512\",\n            \"1024\",\n            \"2048\",\n            \"4096\"\n          ]\n        },\n        \"Memory\": {\n          \"type\": \"string\",\n          \"description\": \"The amount of memory, in MB, reserved for each instance.\",\n          \"enum\": [\n            \"512\",\n            \"1024\",\n            \"2048\",\n            \"3072\",\n            \"4096\",\n            \"\
  6144\",\n            \"8192\",\n            \"10240\",\n            \"12288\"\n          ]\n        },\n        \"InstanceRoleArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of an IAM role that provides permissions to the App Runner service.\"\n        }\n      }\n    },\n    \"AutoScalingConfigurationSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of an auto scaling configuration.\",\n      \"properties\": {\n        \"AutoScalingConfigurationArn\": {\n          \"type\": \"string\"\n        },\n        \"AutoScalingConfigurationName\": {\n          \"type\": \"string\"\n        },\n        \"AutoScalingConfigurationRevision\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"HealthCheckConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the health check configuration for the service.\",\n      \"properties\": {\n        \"Protocol\": {\n          \"type\": \"string\",\n  \
  \        \"enum\": [\n            \"TCP\",\n            \"HTTP\"\n          ]\n        },\n        \"Path\": {\n          \"type\": \"string\"\n        },\n        \"Interval\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 20\n        },\n        \"Timeout\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 20\n        },\n        \"HealthyThreshold\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 20\n        },\n        \"UnhealthyThreshold\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 20\n        }\n      }\n    },\n    \"NetworkConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the networking configuration for the service.\",\n      \"properties\": {\n        \"EgressConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"EgressType\": {\n         \
  \     \"type\": \"string\",\n              \"enum\": [\n                \"DEFAULT\",\n                \"VPC\"\n              ]\n            },\n            \"VpcConnectorArn\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"IngressConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"IsPubliclyAccessible\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"ServiceObservabilityConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the observability configuration of the service.\",\n      \"properties\": {\n        \"ObservabilityEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"ObservabilityConfigurationArn\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: AWS App Runner Service
---
