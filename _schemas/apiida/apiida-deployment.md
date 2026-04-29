---
description: An API deployment operation that provisions a specific API version to one or more managed gateways.
layout: schema
name: APIIDA Deployment
properties_list:
- description: Unique deployment identifier
  name: id
  type: string
- description: Identifier of the API being deployed
  name: apiId
  type: string
- description: Version of the API being deployed
  name: version
  type: string
- description: List of target gateway identifiers
  name: targetGateways
  type: array
- description: Current status of the deployment
  name: status
  type: string
- description: Timestamp when the deployment was initiated
  name: createdAt
  type: string
- description: Timestamp when the deployment completed or failed
  name: completedAt
  type: string
provider_name: APIIDA
provider_slug: apiida
schema_file: json-schema/apiida-deployment.json
slug: apiida-deployment
source_filename: apiida-deployment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"apiida-deployment.json\",\n  \"title\": \"APIIDA Deployment\",\n  \"description\": \"An API deployment operation that provisions a specific API version to one or more managed gateways.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"apiId\", \"version\", \"targetGateways\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique deployment identifier\"\n    },\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the API being deployed\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the API being deployed\"\n    },\n    \"targetGateways\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of target gateway identifiers\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n     \
  \ \"enum\": [\"pending\", \"in_progress\", \"completed\", \"failed\", \"rolled_back\"],\n      \"description\": \"Current status of the deployment\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was initiated\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment completed or failed\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apiida/refs/heads/main/json-schema/apiida-deployment.json
tags:
- API Gateway
- API Management
- Federated API Management
- Governance
- Layer7
title: APIIDA Deployment
---
