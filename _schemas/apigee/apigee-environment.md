---
description: An environment in an Apigee organization. Environments provide a runtime execution context for API proxies, with separate settings for caches, target servers, keystores, and more.
layout: schema
name: Apigee Environment
properties_list:
- description: Required. Name of the environment.
  name: name
  type: string
- description: Display name for the environment.
  name: displayName
  type: string
- description: Description of the environment.
  name: description
  type: string
- description: Output only. State of the environment.
  name: state
  type: string
- description: Output only. Creation time in milliseconds since epoch.
  name: createdAt
  type: string
- description: Output only. Last modification time.
  name: lastModifiedAt
  type: string
- description: Deployment type of the environment.
  name: deploymentType
  type: string
- description: Type of API proxies deployed in this environment.
  name: apiProxyType
  type: string
- description: A collection of key-value property pairs.
  name: properties
  type: object
- description: Runtime node configuration for the environment.
  name: nodeConfig
  type: object
- description: Optional forward proxy URI for the environment.
  name: forwardProxyUri
  type: string
- description: Type of the environment.
  name: type
  type: string
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-environment-schema.json
slug: apigee-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-environment-schema.json\",\n  \"title\": \"Apigee Environment\",\n  \"description\": \"An environment in an Apigee organization. Environments provide a runtime execution context for API proxies, with separate settings for caches, target servers, keystores, and more.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Required. Name of the environment.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the environment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the environment.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. State of the environment.\",\n      \"readOnly\": true,\n      \"enum\": [\"STATE_UNSPECIFIED\", \"CREATING\"\
  , \"ACTIVE\", \"DELETING\", \"UPDATING\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Creation time in milliseconds since epoch.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Last modification time.\",\n      \"readOnly\": true\n    },\n    \"deploymentType\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment type of the environment.\",\n      \"enum\": [\"DEPLOYMENT_TYPE_UNSPECIFIED\", \"PROXY\", \"ARCHIVE\"]\n    },\n    \"apiProxyType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of API proxies deployed in this environment.\",\n      \"enum\": [\"API_PROXY_TYPE_UNSPECIFIED\", \"PROGRAMMABLE\", \"CONFIGURABLE\"]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of key-value property pairs.\",\n      \"properties\": {\n        \"property\": {\n          \"type\"\
  : \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"value\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"nodeConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime node configuration for the environment.\",\n      \"properties\": {\n        \"minNodeCount\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum number of gateway nodes.\"\n        },\n        \"maxNodeCount\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum number of gateway nodes.\"\n        },\n        \"currentAggregateNodeCount\": {\n          \"type\": \"string\",\n          \"description\": \"Output only. Current total number of gateway nodes.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"forwardProxyUri\": {\n      \"type\": \"string\",\n      \"description\": \"Optional\
  \ forward proxy URI for the environment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the environment.\",\n      \"enum\": [\"ENVIRONMENT_TYPE_UNSPECIFIED\", \"BASE\", \"INTERMEDIATE\", \"COMPREHENSIVE\"]\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-environment-schema.json
tags:
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Hybrid
- Integrations
- Microservices
- Monetization
title: Apigee Environment
---
