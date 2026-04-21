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
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-tag-property-schema.json
slug: azure-storage-accounts-tag-property
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: TagProperty
---
