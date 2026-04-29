---
description: Job schema from Azure Container Apps API
layout: schema
name: Job
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-job-schema.json
slug: azure-container-apps-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Job schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\n          \
  \  \"InProgress\",\n            \"Succeeded\",\n            \"Failed\",\n            \"Canceled\",\n            \"Deleting\"\n          ]\n        },\n        \"environmentId\": {\n          \"type\": \"string\"\n        },\n        \"workloadProfileName\": {\n          \"type\": \"string\"\n        },\n        \"configuration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"secrets\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/components/schemas/Secret\"\n              }\n            },\n            \"triggerType\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"Schedule\",\n                \"Event\",\n                \"Manual\"\n              ]\n            },\n            \"replicaTimeout\": {\n              \"type\": \"integer\"\n            },\n            \"replicaRetryLimit\": {\n              \"type\": \"integer\"\n            },\n            \"manualTriggerConfig\"\
  : {\n              \"type\": \"object\",\n              \"properties\": {\n                \"replicaCompletionCount\": {\n                  \"type\": \"integer\"\n                },\n                \"parallelism\": {\n                  \"type\": \"integer\"\n                }\n              }\n            },\n            \"scheduleTriggerConfig\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"cronExpression\": {\n                  \"type\": \"string\"\n                },\n                \"replicaCompletionCount\": {\n                  \"type\": \"integer\"\n                },\n                \"parallelism\": {\n                  \"type\": \"integer\"\n                }\n              }\n            },\n            \"eventTriggerConfig\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"replicaCompletionCount\": {\n                  \"type\": \"integer\"\n                },\n                \"parallelism\"\
  : {\n                  \"type\": \"integer\"\n                },\n                \"scale\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"minExecutions\": {\n                      \"type\": \"integer\"\n                    },\n                    \"maxExecutions\": {\n                      \"type\": \"integer\"\n                    },\n                    \"pollingInterval\": {\n                      \"type\": \"integer\"\n                    },\n                    \"rules\": {\n                      \"type\": \"array\",\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    }\n                  }\n                }\n              }\n            },\n            \"registries\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"server\": {\n       \
  \             \"type\": \"string\"\n                  },\n                  \"username\": {\n                    \"type\": \"string\"\n                  },\n                  \"passwordSecretRef\": {\n                    \"type\": \"string\"\n                  },\n                  \"identity\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"template\": {\n          \"$ref\": \"#/components/schemas/JobExecutionTemplate\"\n        },\n        \"outboundIpAddresses\": {\n          \"type\": \"array\",\n          \"readOnly\": true,\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"eventStreamEndpoint\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-job-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: Job
---
