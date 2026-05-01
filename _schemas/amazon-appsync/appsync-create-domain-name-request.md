---
description: Request to create a custom domain name
layout: schema
name: CreateDomainNameRequest
properties_list:
- description: The custom domain name
  name: domainName
  type: string
- description: ACM certificate ARN
  name: certificateArn
  type: string
- description: Domain name description
  name: description
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-create-domain-name-request-schema.json
slug: appsync-create-domain-name-request
source_filename: appsync-create-domain-name-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-create-domain-name-request-schema.json\",\n  \"title\": \"CreateDomainNameRequest\",\n  \"description\": \"Request to create a custom domain name\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The custom domain name\"\n    },\n    \"certificateArn\": {\n      \"type\": \"string\",\n      \"description\": \"ACM certificate ARN\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Domain name description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-create-domain-name-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: CreateDomainNameRequest
---
