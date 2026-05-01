---
description: A published documentation site in GitBook that serves content from one or more spaces under a configured hostname.
layout: schema
name: GitBook Docs Site
properties_list:
- description: The unique identifier of the docs site.
  name: id
  type: string
- description: The title of the docs site.
  name: title
  type: string
- description: The hostname of the docs site.
  name: hostname
  type: string
- description: URLs associated with the docs site.
  name: urls
  type: object
- description: The timestamp when the docs site was created.
  name: createdAt
  type: string
- description: The timestamp when the docs site was last updated.
  name: updatedAt
  type: string
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/docs-site.json
slug: docs-site
source_filename: docs-site.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/docs-site.json\",\n  \"title\": \"GitBook Docs Site\",\n  \"description\": \"A published documentation site in GitBook that serves content from one or more spaces under a configured hostname.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the docs site.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the docs site.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname of the docs site.\"\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"description\": \"URLs associated with the docs site.\",\n      \"properties\": {\n        \"app\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL\
  \ to the docs site in the GitBook app.\"\n        },\n        \"published\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the published docs site.\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the docs site was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the docs site was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/docs-site.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook Docs Site
---
