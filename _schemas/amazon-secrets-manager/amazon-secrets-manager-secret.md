---
description: Secret schema from Amazon Secrets Manager API
layout: schema
name: Secret
properties_list:
- description: The ARN of the secret.
  name: ARN
  type: string
- description: The friendly name of the secret.
  name: Name
  type: string
- description: The description of the secret.
  name: Description
  type: string
- description: The ARN of the KMS key used to encrypt the secret.
  name: KmsKeyId
  type: string
- description: Whether rotation is enabled for this secret.
  name: RotationEnabled
  type: boolean
- description: The ARN of the Lambda function that rotates the secret.
  name: RotationLambdaARN
  type: string
- description: ''
  name: RotationRules
  type: object
- description: The most recent date and time that rotation was triggered.
  name: LastRotatedDate
  type: string
- description: The last date and time that this secret was modified.
  name: LastChangedDate
  type: string
- description: The last date that this secret was accessed.
  name: LastAccessedDate
  type: string
- description: The date and time the deletion of the secret occurred.
  name: DeletedDate
  type: string
- description: The list of tags attached to the secret.
  name: Tags
  type: array
- description: A list of the versions of the secret that have staging labels attached.
  name: SecretVersionsToStages
  type: object
- description: The name of the service that created this secret.
  name: OwningService
  type: string
- description: The date and time when the secret was created.
  name: CreatedDate
  type: string
- description: The Region the secret is in.
  name: PrimaryRegion
  type: string
provider_name: Amazon Secrets Manager
provider_slug: amazon-secrets-manager
schema_file: json-schema/amazon-secrets-manager-secret-schema.json
slug: amazon-secrets-manager-secret
source_filename: amazon-secrets-manager-secret-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-secret-schema.json\",\n  \"title\": \"Secret\",\n  \"description\": \"Secret schema from Amazon Secrets Manager API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the secret.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name of the secret.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the secret.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the KMS key used to encrypt the secret.\"\n    },\n    \"RotationEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether rotation is enabled for this secret.\"\n    },\n \
  \   \"RotationLambdaARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Lambda function that rotates the secret.\"\n    },\n    \"RotationRules\": {\n      \"$ref\": \"#/components/schemas/RotationRules\"\n    },\n    \"LastRotatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The most recent date and time that rotation was triggered.\"\n    },\n    \"LastChangedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last date and time that this secret was modified.\"\n    },\n    \"LastAccessedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last date that this secret was accessed.\"\n    },\n    \"DeletedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the deletion of the secret occurred.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      },\n      \"description\": \"The list of tags attached to the secret.\"\n    },\n    \"SecretVersionsToStages\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"A list of the versions of the secret that have staging labels attached.\"\n    },\n    \"OwningService\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service that created this secret.\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the secret was created.\"\n    },\n    \"PrimaryRegion\": {\n      \"type\": \"string\",\n      \"description\": \"The Region the secret is in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-secrets-manager/refs/heads/main/json-schema/amazon-secrets-manager-secret-schema.json
tags:
- AWS
- Configuration
- Credentials
- Rotation
- Secrets
- Security
title: Secret
---
