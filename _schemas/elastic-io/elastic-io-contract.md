---
description: Represents a contract (tenant) on the elastic.io iPaaS platform. A contract is the top-level organizational entity that contains workspaces, manages user memberships, controls quota allocations, and defines platform-level settings for an organization.
layout: schema
name: elastic.io Contract
properties_list:
- description: Unique identifier for the contract.
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
schema_file: json-schema/elastic-io-contract.json
slug: elastic-io-contract
source_filename: elastic-io-contract.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/json-schema/elastic-io-contract.json\",\n  \"title\": \"elastic.io Contract\",\n  \"description\": \"Represents a contract (tenant) on the elastic.io iPaaS platform. A contract is the top-level organizational entity that contains workspaces, manages user memberships, controls quota allocations, and defines platform-level settings for an organization.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"attributes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the contract.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"contract\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"required\"\
  : [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the contract.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"active\",\n            \"suspended\",\n            \"terminated\"\n          ],\n          \"description\": \"Current status of the contract.\"\n        },\n        \"flow_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of flows across all workspaces in the contract.\"\n        },\n        \"workspace_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of workspaces in the contract.\"\n        },\n        \"available_roles\": {\n          \"type\": \"array\",\n          \"description\": \"Roles available for assignment within this contract.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n  \
  \            \"id\": {\n                \"type\": \"string\",\n                \"description\": \"Role identifier.\"\n              },\n              \"scope\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"contracts\",\n                  \"workspaces\"\n                ],\n                \"description\": \"Scope at which this role applies.\"\n              },\n              \"role\": {\n                \"type\": \"string\",\n                \"description\": \"Role name.\"\n              }\n            }\n          }\n        },\n        \"support_user_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"User ID of the designated support contact.\"\n        },\n        \"custom_data\": {\n          \"type\": \"object\",\n          \"description\": \"Custom metadata associated with the contract.\",\n          \"additionalProperties\": true\n        },\n        \"created_at\": {\n          \"\
  type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the contract was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the contract was last updated.\"\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"workspaces\": {\n          \"type\": \"object\",\n          \"description\": \"Workspaces belonging to this contract.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"format\": \"uuid\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"const\": \"workspace\"\
  \n                  }\n                }\n              }\n            }\n          }\n        },\n        \"members\": {\n          \"type\": \"object\",\n          \"description\": \"Users who are members of this contract.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"format\": \"uuid\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"const\": \"member\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/elastic-io/refs/heads/main/json-schema/elastic-io-contract.json
tags:
- Integrations
- iPaaS
- SaaS Integration
title: elastic.io Contract
---
