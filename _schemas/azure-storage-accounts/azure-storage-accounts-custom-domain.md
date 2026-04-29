---
description: The custom domain assigned to this storage account. This can be set via Update.
layout: schema
name: CustomDomain
properties_list:
- description: Gets or sets the custom domain name assigned to the storage account. Name is the CNAME source.
  name: name
  type: string
- description: Indicates whether indirect CName validation is enabled. Default value is false. This should only be set on updates.
  name: useSubDomainName
  type: boolean
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-custom-domain-schema.json
slug: azure-storage-accounts-custom-domain
source_filename: azure-storage-accounts-custom-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-custom-domain-schema.json\",\n  \"title\": \"CustomDomain\",\n  \"description\": \"The custom domain assigned to this storage account. This can be set via Update.\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Gets or sets the custom domain name assigned to the storage account. Name is the CNAME source.\",\n      \"type\": \"string\"\n    },\n    \"useSubDomainName\": {\n      \"description\": \"Indicates whether indirect CName validation is enabled. Default value is false. This should only be set on updates.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-custom-domain-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: CustomDomain
---
