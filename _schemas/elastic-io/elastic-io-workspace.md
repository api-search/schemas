---
description: Represents a workspace on the elastic.io iPaaS platform. A workspace is an organizational unit within a contract that contains integration flows, credentials, and team members. Workspaces provide isolation and access control for integration resources.
layout: schema
name: elastic.io Workspace
properties_list:
- description: Unique identifier for the workspace.
  name: id
  type: string
- description: Resource type identifier.
  name: type
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
provider_name: Elastic.io
provider_slug: elastic-io
schema_file: json-schema/elastic-io-workspace.json
slug: elastic-io-workspace
source_filename: elastic-io-workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/json-schema/elastic-io-workspace.json\",\n  \"title\": \"elastic.io Workspace\",\n  \"description\": \"Represents a workspace on the elastic.io iPaaS platform. A workspace is an organizational unit within a contract that contains integration flows, credentials, and team members. Workspaces provide isolation and access control for integration resources.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the workspace.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"workspace\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"required\"\
  : [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the workspace.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Optional description of the workspace's purpose.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"full\",\n            \"limited\"\n          ],\n          \"description\": \"Workspace type controlling available features and quotas.\"\n        },\n        \"flow_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of integration flows in this workspace.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the workspace was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"Timestamp when the workspace was last updated.\"\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contract\": {\n          \"type\": \"object\",\n          \"description\": \"The contract (tenant) this workspace belongs to.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"string\",\n                  \"format\": \"uuid\"\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"const\": \"contract\"\n                }\n              }\n            }\n          }\n        },\n        \"members\": {\n          \"type\": \"object\",\n          \"description\": \"Users who are members of this workspace.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"array\"\
  ,\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"format\": \"uuid\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"const\": \"member\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/json-schema/elastic-io-workspace.json
tags:
- Integrations
- iPaaS
- SaaS Integration
title: elastic.io Workspace
---
