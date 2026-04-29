---
description: The properties of an ImmutabilityPolicy of a blob container.
layout: schema
name: ImmutabilityPolicyProperties
properties_list:
- description: ImmutabilityPolicy Etag.
  name: etag
  type: string
- description: The properties of an ImmutabilityPolicy of a blob container.
  name: properties
  type: object
- description: The ImmutabilityPolicy update history of the blob container.
  name: updateHistory
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-immutability-policy-properties-schema.json
slug: azure-storage-accounts-immutability-policy-properties
source_filename: azure-storage-accounts-immutability-policy-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-immutability-policy-properties-schema.json\",\n  \"title\": \"ImmutabilityPolicyProperties\",\n  \"description\": \"The properties of an ImmutabilityPolicy of a blob container.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"ImmutabilityPolicy Etag.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/ImmutabilityPolicyProperty\",\n      \"description\": \"The properties of an ImmutabilityPolicy of a blob container.\",\n      \"x-ms-client-flatten\": true\n    },\n    \"updateHistory\": {\n      \"description\": \"The ImmutabilityPolicy update history of the blob container.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/UpdateHistoryProperty\"\n      },\n      \"readOnly\": true,\n\
  \      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-immutability-policy-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ImmutabilityPolicyProperties
---
