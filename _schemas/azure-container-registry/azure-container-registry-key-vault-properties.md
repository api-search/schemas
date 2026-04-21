---
description: KeyVaultProperties schema from Azure Container Registry API
layout: schema
name: KeyVaultProperties
properties_list:
- description: The client id of the identity which will be used to access key vault.
  name: identity
  type: string
- description: Key vault uri to access the encryption key.
  name: keyIdentifier
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-key-vault-properties-schema.json
slug: azure-container-registry-key-vault-properties
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: KeyVaultProperties
---
