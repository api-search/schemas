---
description: Paged collection of directory objects
layout: schema
name: DirectoryObjectCollectionResponse
properties_list:
- description: ''
  name: '@odata.context'
  type: string
- description: ''
  name: '@odata.count'
  type: integer
- description: ''
  name: '@odata.nextLink'
  type: string
- description: ''
  name: value
  type: array
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-directory-object-collection-response-schema.json
slug: microsoft-entra-graph-identity-directory-object-collection-response
source_filename: microsoft-entra-graph-identity-directory-object-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DirectoryObjectCollectionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paged collection of directory objects\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\"\n    },\n    \"@odata.count\": {\n      \"type\": \"integer\"\n    },\n    \"@odata.nextLink\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-directory-object-collection-response-schema.json
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
title: DirectoryObjectCollectionResponse
---
