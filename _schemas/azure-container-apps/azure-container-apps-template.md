---
description: Container App versioned application definition.
layout: schema
name: Template
properties_list:
- description: ''
  name: revisionSuffix
  type: string
- description: ''
  name: terminationGracePeriodSeconds
  type: integer
- description: ''
  name: initContainers
  type: array
- description: ''
  name: containers
  type: array
- description: ''
  name: scale
  type: object
- description: ''
  name: volumes
  type: array
- description: ''
  name: serviceBinds
  type: array
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-template-schema.json
slug: azure-container-apps-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-template-schema.json\",\n  \"title\": \"Template\",\n  \"description\": \"Container App versioned application definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionSuffix\": {\n      \"type\": \"string\"\n    },\n    \"terminationGracePeriodSeconds\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"initContainers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Container\"\n      }\n    },\n    \"containers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Container\"\n      }\n    },\n    \"scale\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"minReplicas\": {\n          \"type\": \"integer\"\n        },\n        \"\
  maxReplicas\": {\n          \"type\": \"integer\"\n        },\n        \"rules\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"azureQueue\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"queueName\": {\n                    \"type\": \"string\"\n                  },\n                  \"queueLength\": {\n                    \"type\": \"integer\"\n                  },\n                  \"auth\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"secretRef\": {\n                          \"type\": \"string\"\n                        },\n                        \"triggerParameter\": {\n                          \"type\": \"string\"\
  \n                        }\n                      }\n                    }\n                  }\n                }\n              },\n              \"custom\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\"\n                  },\n                  \"metadata\": {\n                    \"type\": \"object\",\n                    \"additionalProperties\": {\n                      \"type\": \"string\"\n                    }\n                  },\n                  \"auth\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"secretRef\": {\n                          \"type\": \"string\"\n                        },\n                        \"triggerParameter\": {\n                          \"type\": \"string\"\n                        }\n               \
  \       }\n                    }\n                  }\n                }\n              },\n              \"http\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"metadata\": {\n                    \"type\": \"object\",\n                    \"additionalProperties\": {\n                      \"type\": \"string\"\n                    }\n                  },\n                  \"auth\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"secretRef\": {\n                          \"type\": \"string\"\n                        },\n                        \"triggerParameter\": {\n                          \"type\": \"string\"\n                        }\n                      }\n                    }\n                  }\n                }\n              },\n              \"tcp\": {\n                \"type\"\
  : \"object\",\n                \"properties\": {\n                  \"metadata\": {\n                    \"type\": \"object\",\n                    \"additionalProperties\": {\n                      \"type\": \"string\"\n                    }\n                  },\n                  \"auth\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"secretRef\": {\n                          \"type\": \"string\"\n                        },\n                        \"triggerParameter\": {\n                          \"type\": \"string\"\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"volumes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  name\": {\n            \"type\": \"string\"\n          },\n          \"storageType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"AzureFile\",\n              \"EmptyDir\",\n              \"Secret\"\n            ]\n          },\n          \"storageName\": {\n            \"type\": \"string\"\n          },\n          \"secrets\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"secretRef\": {\n                  \"type\": \"string\"\n                },\n                \"path\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"mountOptions\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"serviceBinds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"serviceId\": {\n         \
  \   \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-template-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: Template
---
