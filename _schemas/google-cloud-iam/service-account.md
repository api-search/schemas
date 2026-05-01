---
description: A Google Cloud IAM service account resource used to represent an identity for applications and workloads.
layout: schema
name: ServiceAccount
properties_list:
- description: Resource name of the service account in the format projects/{project}/serviceAccounts/{email}.
  name: name
  type: string
- description: ID of the project that owns the service account.
  name: projectId
  type: string
- description: Unique numeric ID of the service account.
  name: uniqueId
  type: string
- description: Email address of the service account.
  name: email
  type: string
- description: Human-readable name for the service account.
  name: displayName
  type: string
- description: Optional description of the service account.
  name: description
  type: string
- description: Whether the service account is disabled.
  name: disabled
  type: boolean
- description: Entity tag for optimistic concurrency control.
  name: etag
  type: string
- description: OAuth 2.0 client ID for the service account.
  name: oauth2ClientId
  type: string
provider_name: Google Cloud IAM
provider_slug: google-cloud-iam
schema_file: json-schema/service-account.json
slug: service-account
source_filename: service-account.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/json-schema/service-account.json\",\n  \"title\": \"ServiceAccount\",\n  \"description\": \"A Google Cloud IAM service account resource used to represent an identity for applications and workloads.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the service account in the format projects/{project}/serviceAccounts/{email}.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the project that owns the service account.\"\n    },\n    \"uniqueId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique numeric ID of the service account.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the service account.\"\
  \n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the service account.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the service account.\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the service account is disabled.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag for optimistic concurrency control.\"\n    },\n    \"oauth2ClientId\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client ID for the service account.\"\n    }\n  },\n  \"required\": [\"email\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-iam/refs/heads/main/json-schema/service-account.json
tags:
- Access Management
- Google Cloud
- IAM
- Identity
- Permissions
- Security
title: ServiceAccount
---
