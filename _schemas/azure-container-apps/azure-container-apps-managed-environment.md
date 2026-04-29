---
description: ManagedEnvironment schema from Azure Container Apps API
layout: schema
name: ManagedEnvironment
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
schema_file: json-schema/azure-container-apps-managed-environment-schema.json
slug: azure-container-apps-managed-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-managed-environment-schema.json\",\n  \"title\": \"ManagedEnvironment\",\n  \"description\": \"ManagedEnvironment schema from Azure Container Apps API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\"\
  : true,\n          \"enum\": [\n            \"Succeeded\",\n            \"Failed\",\n            \"Canceled\",\n            \"Waiting\",\n            \"InitializationInProgress\",\n            \"InfrastructureSetupInProgress\",\n            \"InfrastructureSetupComplete\",\n            \"ScheduledForDelete\",\n            \"UpgradeRequested\",\n            \"UpgradeFailed\"\n          ]\n        },\n        \"daprAIInstrumentationKey\": {\n          \"type\": \"string\"\n        },\n        \"daprAIConnectionString\": {\n          \"type\": \"string\"\n        },\n        \"vnetConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"internal\": {\n              \"type\": \"boolean\"\n            },\n            \"infrastructureSubnetId\": {\n              \"type\": \"string\"\n            },\n            \"dockerBridgeCidr\": {\n              \"type\": \"string\"\n            },\n            \"platformReservedCidr\": {\n              \"type\": \"\
  string\"\n            },\n            \"platformReservedDnsIP\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"defaultDomain\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"staticIp\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"appLogsConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"destination\": {\n              \"type\": \"string\"\n            },\n            \"logAnalyticsConfiguration\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"customerId\": {\n                  \"type\": \"string\"\n                },\n                \"sharedKey\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"zoneRedundant\": {\n          \"type\": \"boolean\"\n        },\n        \"customDomainConfiguration\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"dnsSuffix\": {\n              \"type\": \"string\"\n            },\n            \"certificateValue\": {\n              \"type\": \"string\",\n              \"format\": \"byte\"\n            },\n            \"certificatePassword\": {\n              \"type\": \"string\"\n            },\n            \"customDomainVerificationId\": {\n              \"type\": \"string\",\n              \"readOnly\": true\n            },\n            \"expirationDate\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"readOnly\": true\n            },\n            \"thumbprint\": {\n              \"type\": \"string\",\n              \"readOnly\": true\n            },\n            \"subjectName\": {\n              \"type\": \"string\",\n              \"readOnly\": true\n            }\n          }\n        },\n        \"workloadProfiles\": {\n          \"type\": \"array\",\n        \
  \  \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"workloadProfileType\": {\n                \"type\": \"string\"\n              },\n              \"minimumCount\": {\n                \"type\": \"integer\"\n              },\n              \"maximumCount\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        },\n        \"infrastructureResourceGroup\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"peerAuthentication\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"mtls\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": {\n                  \"type\": \"boolean\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-apps/refs/heads/main/json-schema/azure-container-apps-managed-environment-schema.json
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: ManagedEnvironment
---
