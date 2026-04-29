---
description: Settings properties for Active Directory (AD).
layout: schema
name: ActiveDirectoryProperties
properties_list:
- description: Specifies the security identifier (SID) for Azure Storage.
  name: azureStorageSid
  type: string
- description: Specifies the domain GUID.
  name: domainGuid
  type: string
- description: Specifies the primary domain that the AD DNS server is authoritative for.
  name: domainName
  type: string
- description: Specifies the security identifier (SID).
  name: domainSid
  type: string
- description: Specifies the Active Directory forest to get.
  name: forestName
  type: string
- description: Specifies the NetBIOS domain name.
  name: netBiosDomainName
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-active-directory-properties-schema.json
slug: azure-storage-accounts-active-directory-properties
source_filename: azure-storage-accounts-active-directory-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-active-directory-properties-schema.json\",\n  \"title\": \"ActiveDirectoryProperties\",\n  \"description\": \"Settings properties for Active Directory (AD).\",\n  \"properties\": {\n    \"azureStorageSid\": {\n      \"description\": \"Specifies the security identifier (SID) for Azure Storage.\",\n      \"type\": \"string\"\n    },\n    \"domainGuid\": {\n      \"description\": \"Specifies the domain GUID.\",\n      \"type\": \"string\"\n    },\n    \"domainName\": {\n      \"description\": \"Specifies the primary domain that the AD DNS server is authoritative for.\",\n      \"type\": \"string\"\n    },\n    \"domainSid\": {\n      \"description\": \"Specifies the security identifier (SID).\",\n      \"type\": \"string\"\n    },\n    \"forestName\": {\n      \"description\"\
  : \"Specifies the Active Directory forest to get.\",\n      \"type\": \"string\"\n    },\n    \"netBiosDomainName\": {\n      \"description\": \"Specifies the NetBIOS domain name.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"domainName\",\n    \"netBiosDomainName\",\n    \"forestName\",\n    \"domainGuid\",\n    \"domainSid\",\n    \"azureStorageSid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-active-directory-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ActiveDirectoryProperties
---
