---
description: VpcConnector schema from AWS App Runner
layout: schema
name: VpcConnector
properties_list:
- description: ''
  name: VpcConnectorName
  type: string
- description: ''
  name: VpcConnectorArn
  type: string
- description: ''
  name: VpcConnectorRevision
  type: integer
- description: ''
  name: Subnets
  type: array
- description: ''
  name: SecurityGroups
  type: array
- description: ''
  name: Status
  type: string
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: DeletedAt
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-vpc-connector-schema.json
slug: app-runner-vpc-connector
source_filename: app-runner-vpc-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcConnectorName\": {\n      \"type\": \"string\"\n    },\n    \"VpcConnectorArn\": {\n      \"type\": \"string\"\n    },\n    \"VpcConnectorRevision\": {\n      \"type\": \"integer\"\n    },\n    \"Subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"SecurityGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n      ]\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"DeletedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-vpc-connector-schema.json\"\
  ,\n  \"title\": \"VpcConnector\",\n  \"description\": \"VpcConnector schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-vpc-connector-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: VpcConnector
---
