---
description: Schema representing an Amazon S3 Glacier vault resource. A vault is a container for storing archives in Amazon S3 Glacier, providing durable and low-cost storage for data archiving and long-term backup.
layout: schema
name: Amazon S3 Glacier Vault
properties_list:
- description: The Amazon Resource Name (ARN) of the vault.
  name: VaultARN
  type: string
- description: The name of the vault.
  name: VaultName
  type: string
- description: The Universal Coordinated Time (UTC) date when the vault was created.
  name: CreationDate
  type: string
- description: The Universal Coordinated Time (UTC) date when Amazon S3 Glacier completed the last vault inventory.
  name: LastInventoryDate
  type: string
- description: The number of archives in the vault as of the last inventory date.
  name: NumberOfArchives
  type: integer
- description: Total size, in bytes, of the archives in the vault as of the last inventory date.
  name: SizeInBytes
  type: integer
- description: ''
  name: VaultAccessPolicy
  type: object
- description: ''
  name: VaultNotificationConfig
  type: object
- description: The tags that are assigned to the vault.
  name: Tags
  type: object
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
schema_file: json-schema/amazon-s3-glacier-vault-schema.json
slug: amazon-s3-glacier-vault
source_filename: amazon-s3-glacier-vault-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://schema.api.io/amazon-s3-glacier/amazon-s3-glacier-vault-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Amazon S3 Glacier Vault\",\n  \"description\": \"Schema representing an Amazon S3 Glacier vault resource. A vault is a container for storing archives in Amazon S3 Glacier, providing durable and low-cost storage for data archiving and long-term backup.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"VaultName\"\n  ],\n  \"properties\": {\n    \"VaultARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the vault.\",\n      \"pattern\": \"^arn:aws:glacier:[a-z0-9-]+:[0-9]{12}:vaults/.+$\"\n    },\n    \"VaultName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the vault.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The Universal Coordinated Time (UTC) date when the vault was created.\"\n    },\n    \"LastInventoryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The Universal Coordinated Time (UTC) date when Amazon S3 Glacier completed the last vault inventory.\"\n    },\n    \"NumberOfArchives\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of archives in the vault as of the last inventory date.\",\n      \"minimum\": 0\n    },\n    \"SizeInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total size, in bytes, of the archives in the vault as of the last inventory date.\",\n      \"minimum\": 0\n    },\n    \"VaultAccessPolicy\": {\n      \"$ref\": \"#/$defs/VaultAccessPolicy\"\n    },\n    \"VaultNotificationConfig\": {\n      \"$ref\": \"#/$defs/VaultNotificationConfig\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"The tags that are assigned to the vault.\",\n      \"\
  additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"VaultAccessPolicy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Policy\": {\n          \"type\": \"string\",\n          \"description\": \"The vault access policy document in JSON format.\"\n        }\n      }\n    },\n    \"VaultNotificationConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"SNSTopic\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Simple Notification Service (Amazon SNS) topic ARN.\"\n        },\n        \"Events\": {\n          \"type\": \"array\",\n          \"description\": \"A list of one or more events for which Amazon S3 Glacier will send a notification to the specified Amazon SNS topic.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ArchiveRetrievalCompleted\",\n              \"InventoryRetrievalCompleted\"\n            ]\n   \
  \       }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-vault-schema.json
tags:
- Archive
- Backup
- Storage
title: Amazon S3 Glacier Vault
---
