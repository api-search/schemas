---
description: Container schema from Azure Container Apps API
layout: schema
name: Container
properties_list:
- description: ''
  name: image
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: command
  type: array
- description: ''
  name: args
  type: array
- description: ''
  name: env
  type: array
- description: ''
  name: resources
  type: object
- description: ''
  name: volumeMounts
  type: array
- description: ''
  name: probes
  type: array
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-container-schema.json
slug: azure-container-apps-container
source_filename: azure-container-apps-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-container-schema.json\",\n  \"title\": \"Container\",\n  \"description\": \"Container schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"command\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"args\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"env\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"secretRef\"\
  : {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cpu\": {\n          \"type\": \"number\"\n        },\n        \"memory\": {\n          \"type\": \"string\"\n        },\n        \"ephemeralStorage\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"volumeMounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"volumeName\": {\n            \"type\": \"string\"\n          },\n          \"mountPath\": {\n            \"type\": \"string\"\n          },\n          \"subPath\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"probes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"failureThreshold\": {\n            \"type\": \"integer\"\n        \
  \  },\n          \"httpGet\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"host\": {\n                \"type\": \"string\"\n              },\n              \"httpHeaders\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": {\n                      \"type\": \"string\"\n                    },\n                    \"value\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              },\n              \"path\": {\n                \"type\": \"string\"\n              },\n              \"port\": {\n                \"type\": \"integer\"\n              },\n              \"scheme\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"HTTP\",\n                  \"HTTPS\"\n                ]\n              }\n            }\n    \
  \      },\n          \"initialDelaySeconds\": {\n            \"type\": \"integer\"\n          },\n          \"periodSeconds\": {\n            \"type\": \"integer\"\n          },\n          \"successThreshold\": {\n            \"type\": \"integer\"\n          },\n          \"tcpSocket\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"host\": {\n                \"type\": \"string\"\n              },\n              \"port\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"terminationGracePeriodSeconds\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\"\n          },\n          \"timeoutSeconds\": {\n            \"type\": \"integer\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"Liveness\",\n              \"Readiness\",\n              \"Startup\"\n            ]\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-container-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: Container
---
