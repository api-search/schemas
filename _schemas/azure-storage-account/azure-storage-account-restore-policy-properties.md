---
description: The blob service properties for blob restore policy
layout: schema
name: RestorePolicyProperties
properties_list:
- description: how long this blob can be restored. It should be great than zero and less than DeleteRetentionPolicy.days.
  name: days
  type: integer
- description: Blob restore is enabled if set to true.
  name: enabled
  type: boolean
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-restore-policy-properties-schema.json
slug: azure-storage-account-restore-policy-properties
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: RestorePolicyProperties
---
