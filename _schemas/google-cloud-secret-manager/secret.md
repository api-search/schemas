---
description: A Google Cloud Secret Manager secret resource representing a logical grouping of secret versions containing sensitive data.
layout: schema
name: Secret
properties_list:
- description: Resource name of the secret in the format projects/{project}/secrets/{secretId}.
  name: name
  type: string
- description: Replication policy of the secret.
  name: replication
  type: object
- description: Timestamp when the secret was created.
  name: createTime
  type: string
- description: Labels attached to the secret.
  name: labels
  type: object
- description: Timestamp at which the secret expires.
  name: expireTime
  type: string
- description: Time-to-live duration for the secret.
  name: ttl
  type: string
- description: Entity tag for optimistic concurrency control.
  name: etag
  type: string
- description: Rotation policy for the secret.
  name: rotation
  type: object
- description: Mapping of alias strings to secret version numbers.
  name: versionAliases
  type: object
- description: Pub/Sub topics for secret event notifications.
  name: topics
  type: array
provider_name: Google Cloud Secret Manager
provider_slug: google-cloud-secret-manager
schema_file: json-schema/secret.json
slug: secret
source_filename: secret.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-secret-manager/refs/heads/main/json-schema/secret.json\",\n  \"title\": \"Secret\",\n  \"description\": \"A Google Cloud Secret Manager secret resource representing a logical grouping of secret versions containing sensitive data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the secret in the format projects/{project}/secrets/{secretId}.\"\n    },\n    \"replication\": {\n      \"type\": \"object\",\n      \"description\": \"Replication policy of the secret.\",\n      \"properties\": {\n        \"automatic\": {\n          \"type\": \"object\",\n          \"description\": \"Automatic replication policy.\",\n          \"properties\": {\n            \"customerManagedEncryption\": {\n              \"type\": \"object\",\n              \"properties\"\
  : {\n                \"kmsKeyName\": {\n                  \"type\": \"string\",\n                  \"description\": \"Resource name of the Cloud KMS key used for encryption.\"\n                }\n              }\n            }\n          }\n        },\n        \"userManaged\": {\n          \"type\": \"object\",\n          \"description\": \"User-managed replication policy.\",\n          \"properties\": {\n            \"replicas\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"location\": {\n                    \"type\": \"string\",\n                    \"description\": \"Cloud region for the replica.\"\n                  },\n                  \"customerManagedEncryption\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"kmsKeyName\": {\n                        \"type\": \"string\"\n                      }\n     \
  \               }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the secret was created.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels attached to the secret.\"\n    },\n    \"expireTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp at which the secret expires.\"\n    },\n    \"ttl\": {\n      \"type\": \"string\",\n      \"description\": \"Time-to-live duration for the secret.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag for optimistic concurrency control.\"\n    },\n    \"rotation\": {\n      \"type\": \"object\",\n      \"description\": \"Rotation policy for the secret.\"\
  ,\n      \"properties\": {\n        \"nextRotationTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the next scheduled rotation.\"\n        },\n        \"rotationPeriod\": {\n          \"type\": \"string\",\n          \"description\": \"Duration between automatic rotations.\"\n        }\n      }\n    },\n    \"versionAliases\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Mapping of alias strings to secret version numbers.\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Pub/Sub topic resource name.\"\n          }\n        }\n      },\n      \"description\": \"Pub/Sub topics for secret event notifications.\"\n    }\n  },\n  \"required\": [\"replication\"\
  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-secret-manager/refs/heads/main/json-schema/secret.json
tags:
- Configuration
- Credentials
- Google Cloud
- Key Management
- Secrets
- Security
title: Secret
---
