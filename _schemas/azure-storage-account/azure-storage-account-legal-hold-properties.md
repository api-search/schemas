---
description: The LegalHold property of a blob container.
layout: schema
name: LegalHoldProperties
properties_list:
- description: 'The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. '
  name: hasLegalHold
  type: boolean
- description: The list of LegalHold tags of a blob container.
  name: tags
  type: array
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-legal-hold-properties-schema.json
slug: azure-storage-account-legal-hold-properties
source_filename: azure-storage-account-legal-hold-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-legal-hold-properties-schema.json\",\n  \"title\": \"LegalHoldProperties\",\n  \"description\": \"The LegalHold property of a blob container.\",\n  \"properties\": {\n    \"hasLegalHold\": {\n      \"description\": \"The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. There can be a maximum of 1000 blob containers with hasLegalHold=true for a given account.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"description\": \"The list of LegalHold tags of a blob container.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/TagProperty\"\n      },\n      \"type\": \"array\"\n    }\n \
  \ },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-legal-hold-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: LegalHoldProperties
---
