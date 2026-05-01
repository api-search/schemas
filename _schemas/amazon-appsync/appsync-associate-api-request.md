---
description: Request to associate an API with a domain name
layout: schema
name: AssociateApiRequest
properties_list:
- description: The API ID to associate
  name: apiId
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-associate-api-request-schema.json
slug: appsync-associate-api-request
source_filename: appsync-associate-api-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-associate-api-request-schema.json\",\n  \"title\": \"AssociateApiRequest\",\n  \"description\": \"Request to associate an API with a domain name\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"The API ID to associate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-associate-api-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: AssociateApiRequest
---
