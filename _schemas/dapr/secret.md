---
description: Represents a secret retrieved from a Dapr secret store. Secrets are returned as key/value string pairs from pluggable stores such as Hashicorp Vault, AWS Secrets Manager, Azure Key Vault, GCP Secret Manager, and Kubernetes Secrets.
layout: schema
name: Dapr Secret
properties_list:
- description: The name of the secret.
  name: name
  type: string
- description: The name of the secret store component.
  name: store
  type: string
- description: The secret key/value pairs.
  name: values
  type: object
- description: Optional metadata for the secret request.
  name: metadata
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/secret.json
slug: secret
source_filename: secret.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/secret.json\",\n  \"title\": \"Dapr Secret\",\n  \"description\": \"Represents a secret retrieved from a Dapr secret store. Secrets are returned as key/value string pairs from pluggable stores such as Hashicorp Vault, AWS Secrets Manager, Azure Key Vault, GCP Secret Manager, and Kubernetes Secrets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the secret.\"\n    },\n    \"store\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the secret store component.\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The secret key/value pairs.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n   \
  \     \"version_id\": {\n          \"type\": \"string\",\n          \"description\": \"Version identifier for the secret.\"\n        },\n        \"version_stage\": {\n          \"type\": \"string\",\n          \"description\": \"Version stage for the secret (e.g., AWSCURRENT).\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace for the secret.\"\n        }\n      },\n      \"description\": \"Optional metadata for the secret request.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/secret.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr Secret
---
