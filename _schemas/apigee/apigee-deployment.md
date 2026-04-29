---
description: Represents a deployment of an API proxy revision to an environment in Apigee. Deployments make API proxies available to receive and process client requests.
layout: schema
name: Apigee Deployment
properties_list:
- description: Environment where the proxy is deployed.
  name: environment
  type: string
- description: API proxy name.
  name: apiProxy
  type: string
- description: API proxy revision number.
  name: revision
  type: string
- description: Time the deployment was initiated.
  name: deployStartTime
  type: string
- description: Current state of the deployment.
  name: state
  type: string
- description: Status reported by individual runtime pods.
  name: pods
  type: array
- description: Conflicts with other deployments sharing the same base path.
  name: routeConflicts
  type: array
provider_name: Apigee
provider_slug: apigee
schema_file: json-schema/apigee-deployment-schema.json
slug: apigee-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/apigee/apigee-deployment-schema.json\",\n  \"title\": \"Apigee Deployment\",\n  \"description\": \"Represents a deployment of an API proxy revision to an environment in Apigee. Deployments make API proxies available to receive and process client requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"Environment where the proxy is deployed.\"\n    },\n    \"apiProxy\": {\n      \"type\": \"string\",\n      \"description\": \"API proxy name.\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"description\": \"API proxy revision number.\"\n    },\n    \"deployStartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time the deployment was initiated.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current\
  \ state of the deployment.\",\n      \"enum\": [\"RUNTIME_STATE_UNSPECIFIED\", \"READY\", \"PROGRESSING\", \"ERROR\"]\n    },\n    \"pods\": {\n      \"type\": \"array\",\n      \"description\": \"Status reported by individual runtime pods.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PodStatus\"\n      }\n    },\n    \"routeConflicts\": {\n      \"type\": \"array\",\n      \"description\": \"Conflicts with other deployments sharing the same base path.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"deployedRevision\": { \"type\": \"string\" },\n          \"environmentGroup\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"PodStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Status of a runtime pod.\",\n      \"properties\": {\n        \"podName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the pod.\"\n        },\n        \"podStatus\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Current status of the pod.\"\n        },\n        \"podStatusTime\": {\n          \"type\": \"string\",\n          \"description\": \"Time the status was last reported.\"\n        },\n        \"deploymentStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Deployment status within the pod.\"\n        },\n        \"deploymentStatusTime\": {\n          \"type\": \"string\",\n          \"description\": \"Time the deployment status was reported.\"\n        },\n        \"deploymentTime\": {\n          \"type\": \"string\",\n          \"description\": \"Time the deployment was last updated in the pod.\"\n        },\n        \"appVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Version of the app running in the pod.\"\n        },\n        \"statusCode\": {\n          \"type\": \"string\",\n          \"description\": \"Status code.\"\n        },\n        \"statusCodeDetails\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Human-readable details for the status code.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/json-schema/apigee-deployment-schema.json
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
title: Apigee Deployment
---
