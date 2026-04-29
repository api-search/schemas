---
description: Represents an encrypted secret for GitHub Actions. The encrypted value is never returned by the API.
layout: schema
name: GitHub Actions Secret
properties_list:
- description: The name of the secret.
  name: name
  type: string
- description: The date and time the secret was created.
  name: created_at
  type: string
- description: The date and time the secret was last updated.
  name: updated_at
  type: string
- description: The visibility scope of the secret (organization secrets only).
  name: visibility
  type: string
- description: The API URL to manage selected repositories for this secret (organization secrets with selected visibility only).
  name: selected_repositories_url
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-secret-schema.json
slug: github-actions-secret
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.github.com/actions/secret.json\",\n  \"title\": \"GitHub Actions Secret\",\n  \"description\": \"Represents an encrypted secret for GitHub Actions. The encrypted value is never returned by the API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the secret.\",\n      \"pattern\": \"^[A-Za-z_][A-Za-z0-9_]*$\",\n      \"examples\": [\"AWS_ACCESS_KEY_ID\", \"NPM_TOKEN\", \"DEPLOY_KEY\"]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the secret was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the secret was last updated.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The visibility scope of the secret (organization secrets only).\",\n      \"enum\": [\"all\", \"private\", \"selected\"]\n    },\n    \"selected_repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL to manage selected repositories for this secret (organization secrets with selected visibility only).\"\n    }\n  },\n  \"required\": [\"name\", \"created_at\", \"updated_at\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-secret-schema.json
tags: []
title: GitHub Actions Secret
---
