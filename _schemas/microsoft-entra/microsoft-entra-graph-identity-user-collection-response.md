---
description: Paged collection of user objects
layout: schema
name: UserCollectionResponse
properties_list:
- description: OData context URL
  name: '@odata.context'
  type: string
- description: Total count of matching resources (if $count=true)
  name: '@odata.count'
  type: integer
- description: URL to retrieve the next page of results
  name: '@odata.nextLink'
  type: string
- description: ''
  name: value
  type: array
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-user-collection-response-schema.json
slug: microsoft-entra-graph-identity-user-collection-response
source_filename: microsoft-entra-graph-identity-user-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCollectionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paged collection of user objects\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\",\n      \"description\": \"OData context URL\"\n    },\n    \"@odata.count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total count of matching resources (if $count=true)\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"URL to retrieve the next page of results\"\n    },\n    \"value\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-user-collection-response-schema.json
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
title: UserCollectionResponse
---
