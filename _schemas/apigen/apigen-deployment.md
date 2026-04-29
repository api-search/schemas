---
description: A deployment record representing an API deployed to a target environment.
layout: schema
name: APIGen Deployment
properties_list:
- description: Unique identifier for the deployment.
  name: id
  type: string
- description: ID of the deployed API.
  name: apiId
  type: string
- description: ID of the parent project.
  name: projectId
  type: string
- description: Target environment for the deployment.
  name: environment
  type: string
- description: Current status of the deployment.
  name: status
  type: string
- description: Live URL of the deployed API, available once deployment succeeds.
  name: url
  type:
  - string
  - 'null'
- description: Version of the API that was deployed.
  name: version
  type: string
- description: Cloud region where the API is deployed.
  name: region
  type: string
- description: Number of running instances.
  name: replicas
  type: integer
- description: Deployment log entries.
  name: logs
  type: array
- description: User ID of the person who initiated the deployment.
  name: deployedBy
  type: string
- description: Timestamp when the deployment was initiated.
  name: createdAt
  type: string
- description: Timestamp when the deployment record was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-deployment-schema.json
slug: apigen-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apigen.com/schemas/deployment.json\",\n  \"title\": \"APIGen Deployment\",\n  \"description\": \"A deployment record representing an API deployed to a target environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the deployment.\"\n    },\n    \"apiId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the deployed API.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the parent project.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"enum\": [\"development\", \"staging\", \"production\"],\n      \"description\": \"Target environment for the deployment.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"\
  enum\": [\"pending\", \"in_progress\", \"deployed\", \"failed\", \"torn_down\"],\n      \"description\": \"Current status of the deployment.\"\n    },\n    \"url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Live URL of the deployed API, available once deployment succeeds.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the API that was deployed.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where the API is deployed.\"\n    },\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"default\": 1,\n      \"description\": \"Number of running instances.\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"\
  level\": {\n            \"type\": \"string\",\n            \"enum\": [\"info\", \"warn\", \"error\"]\n          },\n          \"message\": {\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\"timestamp\", \"level\", \"message\"]\n      },\n      \"description\": \"Deployment log entries.\"\n    },\n    \"deployedBy\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User ID of the person who initiated the deployment.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was initiated.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment record was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"apiId\", \"projectId\", \"environment\", \"status\", \"createdAt\", \"updatedAt\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigen/refs/heads/main/json-schema/apigen-deployment-schema.json
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen Deployment
---
