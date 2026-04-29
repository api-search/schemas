---
description: The App Runner resource that specifies an App Runner endpoint for incoming traffic. It establishes a connection between a VPC interface endpoint and a App Runner service, to make your App Runner service accessible from only within an Amazon VPC.
layout: schema
name: VpcIngressConnection
properties_list:
- description: ''
  name: VpcIngressConnectionArn
  type: object
- description: ''
  name: VpcIngressConnectionName
  type: object
- description: ''
  name: ServiceArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: IngressVpcConfiguration
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: DeletedAt
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-vpcingressconnection-schema.json
slug: amazon-app-runner-vpcingressconnection
source_filename: amazon-app-runner-vpcingressconnection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VpcIngressConnection\",\n  \"description\": \"The App Runner resource that specifies an App Runner endpoint for incoming traffic. It establishes a connection between a VPC interface endpoint and a App Runner service, to make your App Runner service accessible from only within an Amazon VPC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcIngressConnectionArn\": {},\n    \"VpcIngressConnectionName\": {},\n    \"ServiceArn\": {},\n    \"Status\": {},\n    \"AccountId\": {},\n    \"DomainName\": {},\n    \"IngressVpcConfiguration\": {},\n    \"CreatedAt\": {},\n    \"DeletedAt\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-vpcingressconnection-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: VpcIngressConnection
---
