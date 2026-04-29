---
description: The LegalHold property of a blob container.
layout: schema
name: LegalHold
properties_list:
- description: 'The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. '
  name: hasLegalHold
  type: boolean
- description: Each tag should be 3 to 23 alphanumeric characters and is normalized to lower case at SRP.
  name: tags
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-legal-hold-schema.json
slug: azure-storage-accounts-legal-hold
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-legal-hold-schema.json\",\n  \"title\": \"LegalHold\",\n  \"description\": \"The LegalHold property of a blob container.\",\n  \"properties\": {\n    \"hasLegalHold\": {\n      \"description\": \"The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. There can be a maximum of 1000 blob containers with hasLegalHold=true for a given account.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"description\": \"Each tag should be 3 to 23 alphanumeric characters and is normalized to lower case at SRP.\",\n      \"items\": {\n        \"maxLength\": 23,\n        \"minLength\": 3,\n        \"type\"\
  : \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-legal-hold-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: LegalHold
---
