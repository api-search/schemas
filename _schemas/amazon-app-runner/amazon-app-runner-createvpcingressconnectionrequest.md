---
description: ''
layout: schema
name: CreateVpcIngressConnectionRequest
properties_list:
- description: ''
  name: ServiceArn
  type: object
- description: ''
  name: VpcIngressConnectionName
  type: object
- description: ''
  name: IngressVpcConfiguration
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-createvpcingressconnectionrequest-schema.json
slug: amazon-app-runner-createvpcingressconnectionrequest
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateVpcIngressConnectionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceArn\": {},\n    \"VpcIngressConnectionName\": {},\n    \"IngressVpcConfiguration\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"ServiceArn\",\n    \"VpcIngressConnectionName\",\n    \"IngressVpcConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-createvpcingressconnectionrequest-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CreateVpcIngressConnectionRequest
---
