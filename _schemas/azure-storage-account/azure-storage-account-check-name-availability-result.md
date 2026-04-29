---
description: The CheckNameAvailability operation response.
layout: schema
name: CheckNameAvailabilityResult
properties_list:
- description: Gets an error message explaining the Reason value in more detail.
  name: message
  type: string
- description: Gets a boolean value that indicates whether the name is available for you to use. If true, the name is available. If false, the name has already been taken or is invalid and cannot be used.
  name: nameAvailable
  type: boolean
- description: Gets the reason that a storage account name could not be used. The Reason element is only returned if NameAvailable is false.
  name: reason
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-check-name-availability-result-schema.json
slug: azure-storage-account-check-name-availability-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-check-name-availability-result-schema.json\",\n  \"title\": \"CheckNameAvailabilityResult\",\n  \"description\": \"The CheckNameAvailability operation response.\",\n  \"properties\": {\n    \"message\": {\n      \"description\": \"Gets an error message explaining the Reason value in more detail.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"nameAvailable\": {\n      \"description\": \"Gets a boolean value that indicates whether the name is available for you to use. If true, the name is available. If false, the name has already been taken or is invalid and cannot be used.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"reason\": {\n      \"description\": \"Gets the reason that a storage account name could not be used. The Reason\
  \ element is only returned if NameAvailable is false.\",\n      \"enum\": [\n        \"AccountNameInvalid\",\n        \"AlreadyExists\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"Reason\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-check-name-availability-result-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: CheckNameAvailabilityResult
---
