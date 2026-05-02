---
description: A deleted key bundle consisting of a WebKey plus its attributes.
layout: schema
name: DeletedKeyBundle
properties_list:
- description: The url of the recovery object, used to identify and recover the deleted key.
  name: recoveryId
  type: string
- description: The time when the key is scheduled to be purged, in UTC.
  name: scheduledPurgeDate
  type: integer
- description: The time when the key was deleted, in UTC.
  name: deletedDate
  type: integer
provider_name: Azure Key Vault
provider_slug: microsoft-azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-deleted-key-bundle-schema.json
slug: azure-key-vault-data-plane-deleted-key-bundle
source_filename: azure-key-vault-data-plane-deleted-key-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedKeyBundle\",\n  \"type\": \"object\",\n  \"description\": \"A deleted key bundle consisting of a WebKey plus its attributes.\",\n  \"properties\": {\n    \"recoveryId\": {\n      \"type\": \"string\",\n      \"description\": \"The url of the recovery object, used to identify and recover the deleted key.\"\n    },\n    \"scheduledPurgeDate\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the key is scheduled to be purged, in UTC.\"\n    },\n    \"deletedDate\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the key was deleted, in UTC.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-deleted-key-bundle-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: DeletedKeyBundle
---
