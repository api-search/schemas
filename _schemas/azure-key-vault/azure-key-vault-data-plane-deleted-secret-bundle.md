---
description: A deleted secret bundle consisting of its previous id, attributes, tags, and deletion information.
layout: schema
name: DeletedSecretBundle
properties_list:
- description: The url of the recovery object, used to identify and recover the deleted secret.
  name: recoveryId
  type: string
- description: The time when the secret is scheduled to be purged, in UTC.
  name: scheduledPurgeDate
  type: integer
- description: The time when the secret was deleted, in UTC.
  name: deletedDate
  type: integer
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-deleted-secret-bundle-schema.json
slug: azure-key-vault-data-plane-deleted-secret-bundle
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedSecretBundle\",\n  \"type\": \"object\",\n  \"description\": \"A deleted secret bundle consisting of its previous id, attributes, tags, and deletion information.\",\n  \"properties\": {\n    \"recoveryId\": {\n      \"type\": \"string\",\n      \"description\": \"The url of the recovery object, used to identify and recover the deleted secret.\"\n    },\n    \"scheduledPurgeDate\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the secret is scheduled to be purged, in UTC.\"\n    },\n    \"deletedDate\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the secret was deleted, in UTC.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-deleted-secret-bundle-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: DeletedSecretBundle
---
