---
description: VpcDNSTarget schema from AWS App Runner
layout: schema
name: VpcDNSTarget
properties_list:
- description: ''
  name: VpcIngressConnectionArn
  type: string
- description: ''
  name: VpcId
  type: string
- description: ''
  name: DomainName
  type: string
provider_name: AWS App Runner
provider_slug: aws-app-runner
schema_file: json-schema/app-runner-vpc-dns-target-schema.json
slug: app-runner-vpc-dns-target
source_filename: app-runner-vpc-dns-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcIngressConnectionArn\": {\n      \"type\": \"string\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\"\n    },\n    \"DomainName\": {\n      \"type\": \"string\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-vpc-dns-target-schema.json\",\n  \"title\": \"VpcDNSTarget\",\n  \"description\": \"VpcDNSTarget schema from AWS App Runner\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-runner/refs/heads/main/json-schema/app-runner-vpc-dns-target-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Microservices
- Serverless
title: VpcDNSTarget
---
