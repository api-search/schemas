---
description: Response with list of domain names
layout: schema
name: ListDomainNamesResponse
properties_list:
- description: List of domain name configurations
  name: domainNameConfigs
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-list-domain-names-response-schema.json
slug: appsync-list-domain-names-response
source_filename: appsync-list-domain-names-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-list-domain-names-response-schema.json\",\n  \"title\": \"ListDomainNamesResponse\",\n  \"description\": \"Response with list of domain names\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainNameConfigs\": {\n      \"type\": \"array\",\n      \"description\": \"List of domain name configurations\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-list-domain-names-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: ListDomainNamesResponse
---
