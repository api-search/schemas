---
description: Settings for Azure Files identity based authentication.
layout: schema
name: AzureFilesIdentityBasedAuthentication
properties_list:
- description: Required if choose AD.
  name: activeDirectoryProperties
  type: object
- description: Indicates the directory service used.
  name: directoryServiceOptions
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-azure-files-identity-based-authentication-schema.json
slug: azure-storage-account-azure-files-identity-based-authentication
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-azure-files-identity-based-authentication-schema.json\",\n  \"title\": \"AzureFilesIdentityBasedAuthentication\",\n  \"description\": \"Settings for Azure Files identity based authentication.\",\n  \"properties\": {\n    \"activeDirectoryProperties\": {\n      \"$ref\": \"#/definitions/ActiveDirectoryProperties\",\n      \"description\": \"Required if choose AD.\"\n    },\n    \"directoryServiceOptions\": {\n      \"description\": \"Indicates the directory service used.\",\n      \"enum\": [\n        \"None\",\n        \"AADDS\",\n        \"AD\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"DirectoryServiceOptions\"\n      }\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"directoryServiceOptions\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-azure-files-identity-based-authentication-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: AzureFilesIdentityBasedAuthentication
---
