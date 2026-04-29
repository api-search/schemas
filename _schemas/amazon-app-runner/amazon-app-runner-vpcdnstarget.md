---
description: DNS Target record for a custom domain of this Amazon VPC.
layout: schema
name: VpcDNSTarget
properties_list:
- description: ''
  name: VpcIngressConnectionArn
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: DomainName
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-vpcdnstarget-schema.json
slug: amazon-app-runner-vpcdnstarget
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VpcDNSTarget\",\n  \"description\": \"DNS Target record for a custom domain of this Amazon VPC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcIngressConnectionArn\": {},\n    \"VpcId\": {},\n    \"DomainName\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-vpcdnstarget-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: VpcDNSTarget
---
