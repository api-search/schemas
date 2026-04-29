---
description: An Appsmith low-code application
layout: schema
name: Application
properties_list:
- description: Unique application identifier
  name: applicationId
  type: string
- description: Application name
  name: name
  type: string
- description: Application description
  name: description
  type: string
- description: Workspace the application belongs to
  name: workspaceId
  type: string
- description: Whether the application is publicly accessible
  name: isPublic
  type: boolean
- description: Application creation timestamp
  name: createdAt
  type: string
- description: Last modification timestamp
  name: modifiedAt
  type: string
- description: Pages within the application
  name: pages
  type: array
provider_name: Appsmith
provider_slug: appsmith
schema_file: json-schema/application-schema.json
slug: application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appsmith/main/json-schema/application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"An Appsmith low-code application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique application identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Application description\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Workspace the application belongs to\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application is publicly accessible\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Application creation timestamp\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Pages within the application\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\n    \"applicationId\",\n    \"name\",\n    \"workspaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/json-schema/application-schema.json
tags:
- Low-Code
- Open Source
- Internal Tools
- Workflow Automation
- Developer Tools
title: Application
---
