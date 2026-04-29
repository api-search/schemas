---
description: Service schema from AWS App Runner
layout: schema
name: Service
properties_list:
- description: ''
  name: ServiceName
  type: string
- description: ''
  name: ServiceId
  type: string
- description: ''
  name: ServiceArn
  type: string
- description: ''
  name: ServiceUrl
  type: string
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
- description: ''
  name: DeletedAt
  type: string
- description: ''
  name: Status
  type: string
- description: ''
  name: SourceConfiguration
  type: object
- description: ''
  name: InstanceConfiguration
  type: object
- description: ''
  name: HealthCheckConfiguration
  type: object
- description: ''
  name: AutoScalingConfigurationSummary
  type: object
- description: ''
  name: NetworkConfiguration
  type: object
- description: ''
  name: ObservabilityConfiguration
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-service-schema.json
slug: app-runner-service
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"type\": \"string\"\n    },\n    \"ServiceId\": {\n      \"type\": \"string\"\n    },\n    \"ServiceArn\": {\n      \"type\": \"string\"\n    },\n    \"ServiceUrl\": {\n      \"type\": \"string\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"DeletedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATE_FAILED\",\n        \"RUNNING\",\n        \"DELETED\",\n        \"DELETE_FAILED\",\n        \"PAUSED\",\n        \"OPERATION_IN_PROGRESS\"\n      ]\n    },\n    \"SourceConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"CodeRepository\": {\n          \"type\": \"object\",\n          \"properties\": {\n       \
  \     \"RepositoryUrl\": {\n              \"type\": \"string\"\n            },\n            \"SourceCodeVersion\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"BRANCH\"\n                  ]\n                },\n                \"Value\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"CodeConfiguration\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"ConfigurationSource\": {\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"REPOSITORY\",\n                    \"API\"\n                  ]\n                },\n                \"CodeConfigurationValues\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"Runtime\": {\n                      \"\
  type\": \"string\",\n                      \"enum\": [\n                        \"PYTHON_3\",\n                        \"NODEJS_12\",\n                        \"NODEJS_14\",\n                        \"NODEJS_16\",\n                        \"NODEJS_18\",\n                        \"CORRETTO_8\",\n                        \"CORRETTO_11\",\n                        \"GO_1\",\n                        \"DOTNET_6\",\n                        \"PHP_81\",\n                        \"RUBY_31\"\n                      ]\n                    },\n                    \"BuildCommand\": {\n                      \"type\": \"string\"\n                    },\n                    \"StartCommand\": {\n                      \"type\": \"string\"\n                    },\n                    \"Port\": {\n                      \"type\": \"string\"\n                    },\n                    \"RuntimeEnvironmentVariables\": {\n                      \"type\": \"object\",\n                      \"additionalProperties\"\
  : {\n                        \"type\": \"string\"\n                      }\n                    },\n                    \"RuntimeEnvironmentSecrets\": {\n                      \"type\": \"object\",\n                      \"additionalProperties\": {\n                        \"type\": \"string\"\n                      }\n                    }\n                  }\n                }\n              }\n            },\n            \"SourceDirectory\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"ImageRepository\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ImageIdentifier\": {\n              \"type\": \"string\"\n            },\n            \"ImageConfiguration\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"RuntimeEnvironmentVariables\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"type\": \"string\"\
  \n                  }\n                },\n                \"RuntimeEnvironmentSecrets\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": {\n                    \"type\": \"string\"\n                  }\n                },\n                \"StartCommand\": {\n                  \"type\": \"string\"\n                },\n                \"Port\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"ImageRepositoryType\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"ECR\",\n                \"ECR_PUBLIC\"\n              ]\n            }\n          }\n        },\n        \"AutoDeploymentsEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"AuthenticationConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ConnectionArn\": {\n              \"type\": \"string\"\n            },\n            \"AccessRoleArn\"\
  : {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"InstanceConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Cpu\": {\n          \"type\": \"string\",\n          \"description\": \"CPU units (e.g., 1024 for 1 vCPU, 256, 512, 1024, 2048, 4096).\"\n        },\n        \"Memory\": {\n          \"type\": \"string\",\n          \"description\": \"Memory in MB (e.g., 2048 for 2 GB).\"\n        },\n        \"InstanceRoleArn\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"HealthCheckConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Protocol\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"TCP\",\n            \"HTTP\"\n          ]\n        },\n        \"Path\": {\n          \"type\": \"string\"\n        },\n        \"Interval\": {\n          \"type\": \"integer\",\n          \"description\": \"Interval in seconds between health\
  \ checks.\"\n        },\n        \"Timeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Timeout in seconds for each health check.\"\n        },\n        \"HealthyThreshold\": {\n          \"type\": \"integer\"\n        },\n        \"UnhealthyThreshold\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"AutoScalingConfigurationSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"AutoScalingConfigurationArn\": {\n          \"type\": \"string\"\n        },\n        \"AutoScalingConfigurationName\": {\n          \"type\": \"string\"\n        },\n        \"AutoScalingConfigurationRevision\": {\n          \"type\": \"integer\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ACTIVE\",\n            \"INACTIVE\"\n          ]\n        },\n        \"CreatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"HasAssociatedService\"\
  : {\n          \"type\": \"boolean\"\n        },\n        \"IsDefault\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"NetworkConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"EgressConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"EgressType\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"DEFAULT\",\n                \"VPC\"\n              ]\n            },\n            \"VpcConnectorArn\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"IngressConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"IsPubliclyAccessible\": {\n              \"type\": \"boolean\"\n            }\n          }\n        },\n        \"IpAddressType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"IPV4\",\n            \"DUAL_STACK\"\n          ]\n        }\n    \
  \  }\n    },\n    \"ObservabilityConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ObservabilityEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"ObservabilityConfigurationArn\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"EncryptionConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"KmsKey\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Service schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-service-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: Service
---
