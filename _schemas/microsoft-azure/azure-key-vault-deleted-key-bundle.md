---
description: A deleted key bundle.
layout: schema
name: DeletedKeyBundle
properties_list:
- description: The URL of the recovery object.
  name: recoveryId
  type: string
- description: The time when the key is scheduled to be purged (Unix time).
  name: scheduledPurgeDate
  type: integer
- description: The time when the key was deleted (Unix time).
  name: deletedDate
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-key-vault-deleted-key-bundle-schema.json
slug: azure-key-vault-deleted-key-bundle
source_filename: azure-key-vault-deleted-key-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeletedKeyBundle\",\n  \"type\": \"object\",\n  \"description\": \"A deleted key bundle.\",\n  \"properties\": {\n    \"recoveryId\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the recovery object.\"\n    },\n    \"scheduledPurgeDate\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the key is scheduled to be purged (Unix time).\"\n    },\n    \"deletedDate\": {\n      \"type\": \"integer\",\n      \"description\": \"The time when the key was deleted (Unix time).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-key-vault-deleted-key-bundle-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeletedKeyBundle
---
