---
description: The LegalHold property of a blob container.
layout: schema
name: LegalHold
properties_list:
- description: 'The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. '
  name: hasLegalHold
  type: boolean
- description: Each tag should be 3 to 23 alphanumeric characters and is normalized to lower case at SRP.
  name: tags
  type: array
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-legal-hold-schema.json
slug: azure-storage-accounts-legal-hold
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: LegalHold
---
