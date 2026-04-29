---
description: The parameters to list SAS credentials of a storage account.
layout: schema
name: AccountSasParameters
properties_list:
- description: The key to sign the account SAS token with.
  name: keyToSign
  type: string
- description: The time at which the shared access signature becomes invalid.
  name: signedExpiry
  type: string
- description: An IP address or a range of IP addresses from which to accept requests.
  name: signedIp
  type: string
- description: 'The signed permissions for the account SAS. Possible values include: Read (r), Write (w), Delete (d), List (l), Add (a), Create (c), Update (u) and Process (p).'
  name: signedPermission
  type: string
- description: The protocol permitted for a request made with the account SAS.
  name: signedProtocol
  type: string
- description: 'The signed resource types that are accessible with the account SAS. Service (s): Access to service-level APIs; Container (c): Access to container-level APIs; Object (o): Access to object-level APIs fo'
  name: signedResourceTypes
  type: string
- description: 'The signed services accessible with the account SAS. Possible values include: Blob (b), Queue (q), Table (t), File (f).'
  name: signedServices
  type: string
- description: The time at which the SAS becomes valid.
  name: signedStart
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-account-sas-parameters-schema.json
slug: azure-storage-accounts-account-sas-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-account-sas-parameters-schema.json\",\n  \"title\": \"AccountSasParameters\",\n  \"description\": \"The parameters to list SAS credentials of a storage account.\",\n  \"properties\": {\n    \"keyToSign\": {\n      \"description\": \"The key to sign the account SAS token with.\",\n      \"type\": \"string\"\n    },\n    \"signedExpiry\": {\n      \"description\": \"The time at which the shared access signature becomes invalid.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"SharedAccessExpiryTime\"\n    },\n    \"signedIp\": {\n      \"description\": \"An IP address or a range of IP addresses from which to accept requests.\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"IPAddressOrRange\"\n    },\n    \"signedPermission\"\
  : {\n      \"description\": \"The signed permissions for the account SAS. Possible values include: Read (r), Write (w), Delete (d), List (l), Add (a), Create (c), Update (u) and Process (p).\",\n      \"enum\": [\n        \"r\",\n        \"d\",\n        \"w\",\n        \"l\",\n        \"a\",\n        \"c\",\n        \"u\",\n        \"p\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"Permissions\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"Permissions\"\n      }\n    },\n    \"signedProtocol\": {\n      \"description\": \"The protocol permitted for a request made with the account SAS.\",\n      \"enum\": [\n        \"https,http\",\n        \"https\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"Protocols\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"HttpProtocol\"\n      }\n    },\n    \"signedResourceTypes\": {\n      \"description\": \"The signed resource types that\
  \ are accessible with the account SAS. Service (s): Access to service-level APIs; Container (c): Access to container-level APIs; Object (o): Access to object-level APIs for blobs, queue messages, table entities, and files.\",\n      \"enum\": [\n        \"s\",\n        \"c\",\n        \"o\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"ResourceTypes\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"SignedResourceTypes\"\n      }\n    },\n    \"signedServices\": {\n      \"description\": \"The signed services accessible with the account SAS. Possible values include: Blob (b), Queue (q), Table (t), File (f).\",\n      \"enum\": [\n        \"b\",\n        \"q\",\n        \"t\",\n        \"f\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"Services\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"Services\"\n      }\n    },\n    \"signedStart\": {\n      \"description\": \"The time\
  \ at which the SAS becomes valid.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"SharedAccessStartTime\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"signedServices\",\n    \"signedResourceTypes\",\n    \"signedPermission\",\n    \"signedExpiry\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-account-sas-parameters-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: AccountSasParameters
---
