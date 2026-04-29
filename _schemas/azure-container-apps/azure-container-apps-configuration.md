---
description: Non-versioned Container App configuration properties.
layout: schema
name: Configuration
properties_list:
- description: ''
  name: secrets
  type: array
- description: ''
  name: activeRevisionsMode
  type: string
- description: ''
  name: ingress
  type: object
- description: ''
  name: registries
  type: array
- description: ''
  name: dapr
  type: object
- description: ''
  name: maxInactiveRevisions
  type: integer
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-configuration-schema.json
slug: azure-container-apps-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-configuration-schema.json\",\n  \"title\": \"Configuration\",\n  \"description\": \"Non-versioned Container App configuration properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"secrets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Secret\"\n      }\n    },\n    \"activeRevisionsMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Multiple\",\n        \"Single\"\n      ]\n    },\n    \"ingress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fqdn\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"external\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"targetPort\": {\n          \"type\": \"integer\"\
  \n        },\n        \"exposedPort\": {\n          \"type\": \"integer\"\n        },\n        \"transport\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"auto\",\n            \"http\",\n            \"http2\",\n            \"tcp\"\n          ],\n          \"default\": \"auto\"\n        },\n        \"traffic\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"revisionName\": {\n                \"type\": \"string\"\n              },\n              \"weight\": {\n                \"type\": \"integer\"\n              },\n              \"latestRevision\": {\n                \"type\": \"boolean\"\n              },\n              \"label\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"customDomains\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"bindingType\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"Disabled\",\n                  \"SniEnabled\"\n                ]\n              },\n              \"certificateId\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"allowInsecure\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"ipSecurityRestrictions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"description\": {\n                \"type\": \"string\"\n              },\n              \"ipAddressRange\": {\n                \"type\": \"string\"\n              },\n              \"action\": {\n            \
  \    \"type\": \"string\",\n                \"enum\": [\n                  \"Allow\",\n                  \"Deny\"\n                ]\n              }\n            }\n          }\n        },\n        \"stickySessions\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"affinity\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"sticky\",\n                \"none\"\n              ]\n            }\n          }\n        },\n        \"clientCertificateMode\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"accept\",\n            \"require\",\n            \"ignore\"\n          ]\n        },\n        \"corsPolicy\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"allowedOrigins\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"allowedMethods\": {\n              \"type\"\
  : \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"allowedHeaders\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"exposeHeaders\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"maxAge\": {\n              \"type\": \"integer\"\n            },\n            \"allowCredentials\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"registries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"server\": {\n            \"type\": \"string\"\n          },\n          \"username\": {\n            \"type\": \"string\"\n          },\n          \"passwordSecretRef\": {\n            \"type\": \"\
  string\"\n          },\n          \"identity\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"dapr\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\"\n        },\n        \"appId\": {\n          \"type\": \"string\"\n        },\n        \"appProtocol\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"http\",\n            \"grpc\"\n          ]\n        },\n        \"appPort\": {\n          \"type\": \"integer\"\n        },\n        \"httpReadBufferSize\": {\n          \"type\": \"integer\"\n        },\n        \"httpMaxRequestSize\": {\n          \"type\": \"integer\"\n        },\n        \"logLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"info\",\n            \"debug\",\n            \"warn\",\n            \"error\"\n          ]\n        },\n        \"enableApiLogging\": {\n          \"type\": \"boolean\"\n        }\n      }\n\
  \    },\n    \"maxInactiveRevisions\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-configuration-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: Configuration
---
