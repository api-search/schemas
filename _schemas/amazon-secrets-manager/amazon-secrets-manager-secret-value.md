---
description: SecretValue schema from Amazon Secrets Manager API
layout: schema
name: SecretValue
properties_list:
- description: The ARN of the secret.
  name: ARN
  type: string
- description: The friendly name of the secret.
  name: Name
  type: string
- description: The unique identifier of this version of the secret.
  name: VersionId
  type: string
- description: The decrypted secret value in binary format.
  name: SecretBinary
  type: string
- description: The decrypted secret value in string format.
  name: SecretString
  type: string
- description: A list of the staging labels that are attached to this version.
  name: VersionStages
  type: array
- description: The date and time that this version of the secret was created.
  name: CreatedDate
  type: string
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
schema_file: json-schema/amazon-secrets-manager-secret-value-schema.json
slug: amazon-secrets-manager-secret-value
source_filename: amazon-secrets-manager-secret-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-secret-value-schema.json\",\n  \"title\": \"SecretValue\",\n  \"description\": \"SecretValue schema from Amazon Secrets Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the secret.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name of the secret.\"\n    },\n    \"VersionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this version of the secret.\"\n    },\n    \"SecretBinary\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"description\": \"The decrypted secret value in binary format.\"\n    },\n    \"SecretString\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The decrypted secret value in string format.\"\n    },\n    \"VersionStages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of the staging labels that are attached to this version.\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that this version of the secret was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-secret-value-schema.json
tags:
- AWS
- Configuration
- Credentials
- Rotation
- Secrets
- Security
title: SecretValue
---
