---
description: Configuration for a custom domain name
layout: schema
name: DomainNameConfig
properties_list:
- description: The custom domain name
  name: domainName
  type: string
- description: Domain name description
  name: description
  type: string
- description: ACM certificate ARN
  name: certificateArn
  type: string
- description: AppSync CNAME for DNS setup
  name: appsyncDomainName
  type: string
- description: Route 53 hosted zone ID
  name: hostedZoneId
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-domain-name-config-schema.json
slug: appsync-domain-name-config
source_filename: appsync-domain-name-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-domain-name-config-schema.json\",\n  \"title\": \"DomainNameConfig\",\n  \"description\": \"Configuration for a custom domain name\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The custom domain name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Domain name description\"\n    },\n    \"certificateArn\": {\n      \"type\": \"string\",\n      \"description\": \"ACM certificate ARN\"\n    },\n    \"appsyncDomainName\": {\n      \"type\": \"string\",\n      \"description\": \"AppSync CNAME for DNS setup\"\n    },\n    \"hostedZoneId\": {\n      \"type\": \"string\",\n      \"description\": \"Route 53 hosted zone ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-domain-name-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: DomainNameConfig
---
