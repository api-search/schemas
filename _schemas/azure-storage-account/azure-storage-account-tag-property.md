---
description: A tag of the LegalHold of a blob container.
layout: schema
name: TagProperty
properties_list:
- description: Returns the Object ID of the user who added the tag.
  name: objectIdentifier
  type: string
- description: The tag value.
  name: tag
  type: string
- description: Returns the Tenant ID that issued the token for the user who added the tag.
  name: tenantId
  type: string
- description: Returns the date and time the tag was added.
  name: timestamp
  type: string
- description: Returns the User Principal Name of the user who added the tag.
  name: upn
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-tag-property-schema.json
slug: azure-storage-account-tag-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-tag-property-schema.json\",\n  \"title\": \"TagProperty\",\n  \"description\": \"A tag of the LegalHold of a blob container.\",\n  \"properties\": {\n    \"objectIdentifier\": {\n      \"description\": \"Returns the Object ID of the user who added the tag.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"description\": \"The tag value.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"tenantId\": {\n      \"description\": \"Returns the Tenant ID that issued the token for the user who added the tag.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"description\": \"Returns the date and time the tag was added.\",\n      \"format\": \"date-time\",\n      \"readOnly\"\
  : true,\n      \"type\": \"string\"\n    },\n    \"upn\": {\n      \"description\": \"Returns the User Principal Name of the user who added the tag.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-tag-property-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: TagProperty
---
