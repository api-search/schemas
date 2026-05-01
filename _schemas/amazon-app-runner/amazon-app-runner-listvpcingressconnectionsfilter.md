---
description: Returns a list of VPC Ingress Connections based on the filter provided. It can return either <code>ServiceArn</code> or <code>VpcEndpointId</code>, or both.
layout: schema
name: ListVpcIngressConnectionsFilter
properties_list:
- description: ''
  name: ServiceArn
  type: object
- description: ''
  name: VpcEndpointId
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-listvpcingressconnectionsfilter-schema.json
slug: amazon-app-runner-listvpcingressconnectionsfilter
source_filename: amazon-app-runner-listvpcingressconnectionsfilter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListVpcIngressConnectionsFilter\",\n  \"description\": \"Returns a list of VPC Ingress Connections based on the filter provided. It can return either <code>ServiceArn</code> or <code>VpcEndpointId</code>, or both.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceArn\": {},\n    \"VpcEndpointId\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-listvpcingressconnectionsfilter-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ListVpcIngressConnectionsFilter
---
