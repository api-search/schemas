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
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-check-name-availability-result-schema.json
slug: azure-storage-accounts-check-name-availability-result
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: CheckNameAvailabilityResult
---
