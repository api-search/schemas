---
description: An update history of the ImmutabilityPolicy of a blob container.
layout: schema
name: UpdateHistoryProperty
properties_list:
- description: The immutability period for the blobs in the container since the policy creation, in days.
  name: immutabilityPeriodSinceCreationInDays
  type: integer
- description: Returns the Object ID of the user who updated the ImmutabilityPolicy.
  name: objectIdentifier
  type: string
- description: Returns the Tenant ID that issued the token for the user who updated the ImmutabilityPolicy.
  name: tenantId
  type: string
- description: Returns the date and time the ImmutabilityPolicy was updated.
  name: timestamp
  type: string
- description: 'The ImmutabilityPolicy update type of a blob container, possible values include: put, lock and extend.'
  name: update
  type: string
- description: Returns the User Principal Name of the user who updated the ImmutabilityPolicy.
  name: upn
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-update-history-property-schema.json
slug: azure-storage-accounts-update-history-property
source_filename: azure-storage-accounts-update-history-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-update-history-property-schema.json\",\n  \"title\": \"UpdateHistoryProperty\",\n  \"description\": \"An update history of the ImmutabilityPolicy of a blob container.\",\n  \"properties\": {\n    \"immutabilityPeriodSinceCreationInDays\": {\n      \"description\": \"The immutability period for the blobs in the container since the policy creation, in days.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"objectIdentifier\": {\n      \"description\": \"Returns the Object ID of the user who updated the ImmutabilityPolicy.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"tenantId\": {\n      \"description\": \"Returns the Tenant ID that issued the token for the user who updated the ImmutabilityPolicy.\",\n      \"readOnly\": true,\n\
  \      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"description\": \"Returns the date and time the ImmutabilityPolicy was updated.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"update\": {\n      \"description\": \"The ImmutabilityPolicy update type of a blob container, possible values include: put, lock and extend.\",\n      \"enum\": [\n        \"put\",\n        \"lock\",\n        \"extend\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ImmutabilityPolicyUpdateType\"\n      }\n    },\n    \"upn\": {\n      \"description\": \"Returns the User Principal Name of the user who updated the ImmutabilityPolicy.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-update-history-property-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: UpdateHistoryProperty
---
