---
description: The configuration of your VPC and the associated VPC endpoint. The VPC endpoint is an Amazon Web Services PrivateLink resource that allows access to your App Runner services from within an Amazon VPC.
layout: schema
name: IngressVpcConfiguration
properties_list:
- description: ''
  name: VpcId
  type: object
- description: ''
  name: VpcEndpointId
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-ingressvpcconfiguration-schema.json
slug: amazon-app-runner-ingressvpcconfiguration
source_filename: amazon-app-runner-ingressvpcconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"IngressVpcConfiguration\",\n  \"description\": \"The configuration of your VPC and the associated VPC endpoint. The VPC endpoint is an Amazon Web Services PrivateLink resource that allows access to your App Runner services from within an Amazon VPC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcId\": {},\n    \"VpcEndpointId\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-ingressvpcconfiguration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: IngressVpcConfiguration
---
