---
description: The properties of the Azure File volume. Azure File shares are mounted as volumes.
layout: schema
name: AzureFileVolume
properties_list:
- description: The flag indicating whether the Azure File shared mounted as a volume is read-only.
  name: readOnly
  type: boolean
- description: The name of the Azure File share to be mounted as a volume.
  name: shareName
  type: string
- description: The storage account access key used to access the Azure File share.
  name: storageAccountKey
  type: string
- description: The name of the storage account that contains the Azure File share.
  name: storageAccountName
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-azure-file-volume-schema.json
slug: azure-container-instances-azure-file-volume
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: AzureFileVolume
---
