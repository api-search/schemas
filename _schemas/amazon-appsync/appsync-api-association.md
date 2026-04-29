---
description: An association between a custom domain name and a GraphQL API
layout: schema
name: ApiAssociation
properties_list:
- description: The custom domain name
  name: domainName
  type: string
- description: The API ID
  name: apiId
  type: string
- description: The association status
  name: associationStatus
  type: string
- description: Details about the deployment
  name: deploymentDetail
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-api-association-schema.json
slug: appsync-api-association
source_filename: appsync-api-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-api-association-schema.json\",\n  \"title\": \"ApiAssociation\",\n  \"description\": \"An association between a custom domain name and a GraphQL API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The custom domain name\"\n    },\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"The API ID\"\n    },\n    \"associationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The association status\"\n    },\n    \"deploymentDetail\": {\n      \"type\": \"string\",\n      \"description\": \"Details about the deployment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-api-association-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: ApiAssociation
---
