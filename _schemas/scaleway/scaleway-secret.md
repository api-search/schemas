---
description: A secret stored in Scaleway Secret Manager
layout: schema
name: Scaleway Secret
properties_list:
- description: Unique identifier of the secret
  name: id
  type: string
- description: Name of the secret (must be unique within a project)
  name: name
  type: string
- description: Current status of the secret
  name: status
  type: string
- description: Project ID the secret belongs to
  name: project_id
  type: string
- description: Organization ID that owns the secret
  name: organization_id
  type: string
- description: Region where the secret is stored
  name: region
  type: string
- description: User-defined tags for the secret
  name: tags
  type: array
- description: Human-readable description of the secret
  name: description
  type: string
- description: Type of secret being stored
  name: type
  type: string
- description: Number of versions of this secret
  name: version_count
  type: integer
- description: Whether the secret is managed by Scaleway
  name: is_managed
  type: boolean
- description: Path for organizing secrets in a hierarchy
  name: path
  type: string
- description: Timestamp when the secret was created
  name: created_at
  type: string
- description: Timestamp when the secret was last updated
  name: updated_at
  type: string
provider_name: Scaleway
provider_slug: scaleway
schema_file: json-schema/scaleway-secret-schema.json
slug: scaleway-secret
source_filename: scaleway-secret-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scaleway/main/json-schema/scaleway-secret-schema.json\",\n  \"title\": \"Scaleway Secret\",\n  \"description\": \"A secret stored in Scaleway Secret Manager\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\", \"project_id\", \"region\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the secret\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the secret (must be unique within a project)\",\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\",\n      \"maxLength\": 255\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ready\", \"locked\"],\n      \"description\": \"Current status of the secret\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"format\": \"\
  uuid\",\n      \"description\": \"Project ID the secret belongs to\"\n    },\n    \"organization_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Organization ID that owns the secret\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region where the secret is stored\",\n      \"examples\": [\"fr-par\", \"nl-ams\", \"pl-waw\"]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined tags for the secret\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the secret\",\n      \"maxLength\": 1000\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown_secret_type\", \"opaque\", \"certificate\", \"key_value\", \"basic_credentials\", \"database_credentials\", \"ssh_key\"],\n      \"description\": \"Type of secret being stored\"\n \
  \   },\n    \"version_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of versions of this secret\"\n    },\n    \"is_managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the secret is managed by Scaleway\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path for organizing secrets in a hierarchy\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the secret was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the secret was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/json-schema/scaleway-secret-schema.json
tags:
- AI
- Cloud Computing
- Containers
- Database
- European Cloud
- Infrastructure
- Kubernetes
- Serverless
- Storage
title: Scaleway Secret
---
