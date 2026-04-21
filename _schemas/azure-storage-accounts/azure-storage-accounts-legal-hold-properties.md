---
description: The LegalHold property of a blob container.
layout: schema
name: LegalHoldProperties
properties_list:
- description: 'The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. '
  name: hasLegalHold
  type: boolean
- description: The list of LegalHold tags of a blob container.
  name: tags
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-legal-hold-properties-schema.json
slug: azure-storage-accounts-legal-hold-properties
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: LegalHoldProperties
---
