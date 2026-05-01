---
description: ''
layout: schema
name: CreateVpcConnectorRequest
properties_list:
- description: ''
  name: VpcConnectorName
  type: object
- description: ''
  name: Subnets
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-createvpcconnectorrequest-schema.json
slug: amazon-app-runner-createvpcconnectorrequest
source_filename: amazon-app-runner-createvpcconnectorrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateVpcConnectorRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcConnectorName\": {},\n    \"Subnets\": {},\n    \"SecurityGroups\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"VpcConnectorName\",\n    \"Subnets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-createvpcconnectorrequest-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CreateVpcConnectorRequest
---
