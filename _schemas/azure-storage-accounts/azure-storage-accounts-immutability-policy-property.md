---
description: The properties of an ImmutabilityPolicy of a blob container.
layout: schema
name: ImmutabilityPolicyProperty
properties_list:
- description: The immutability period for the blobs in the container since the policy creation, in days.
  name: immutabilityPeriodSinceCreationInDays
  type: integer
- description: 'The ImmutabilityPolicy state of a blob container, possible values include: Locked and Unlocked.'
  name: state
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-immutability-policy-property-schema.json
slug: azure-storage-accounts-immutability-policy-property
source_filename: azure-storage-accounts-immutability-policy-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-immutability-policy-property-schema.json\",\n  \"title\": \"ImmutabilityPolicyProperty\",\n  \"description\": \"The properties of an ImmutabilityPolicy of a blob container.\",\n  \"properties\": {\n    \"immutabilityPeriodSinceCreationInDays\": {\n      \"description\": \"The immutability period for the blobs in the container since the policy creation, in days.\",\n      \"type\": \"integer\"\n    },\n    \"state\": {\n      \"description\": \"The ImmutabilityPolicy state of a blob container, possible values include: Locked and Unlocked.\",\n      \"enum\": [\n        \"Locked\",\n        \"Unlocked\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ImmutabilityPolicyState\"\n \
  \     }\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"immutabilityPeriodSinceCreationInDays\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-immutability-policy-property-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ImmutabilityPolicyProperty
---
