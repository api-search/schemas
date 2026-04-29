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
source_filename: azure-container-instances-azure-file-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-azure-file-volume-schema.json\",\n  \"title\": \"AzureFileVolume\",\n  \"description\": \"The properties of the Azure File volume. Azure File shares are mounted as volumes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"readOnly\": {\n      \"description\": \"The flag indicating whether the Azure File shared mounted as a volume is read-only.\",\n      \"type\": \"boolean\"\n    },\n    \"shareName\": {\n      \"description\": \"The name of the Azure File share to be mounted as a volume.\",\n      \"type\": \"string\"\n    },\n    \"storageAccountKey\": {\n      \"description\": \"The storage account access key used to access the Azure File share.\",\n      \"type\": \"string\"\n    },\n    \"storageAccountName\": {\n      \"description\": \"The name of the storage\
  \ account that contains the Azure File share.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"shareName\",\n    \"storageAccountName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-azure-file-volume-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: AzureFileVolume
---
