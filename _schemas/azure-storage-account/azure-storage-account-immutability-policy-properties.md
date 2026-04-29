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
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-immutability-policy-properties-schema.json
slug: azure-storage-account-immutability-policy-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-immutability-policy-properties-schema.json\",\n  \"title\": \"ImmutabilityPolicyProperties\",\n  \"description\": \"The properties of an ImmutabilityPolicy of a blob container.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"ImmutabilityPolicy Etag.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/ImmutabilityPolicyProperty\",\n      \"description\": \"The properties of an ImmutabilityPolicy of a blob container.\",\n      \"x-ms-client-flatten\": true\n    },\n    \"updateHistory\": {\n      \"description\": \"The ImmutabilityPolicy update history of the blob container.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/UpdateHistoryProperty\"\n      },\n      \"readOnly\": true,\n\
  \      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-immutability-policy-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ImmutabilityPolicyProperties
---
