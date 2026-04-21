---
description: Properties of an artifact source.
layout: schema
name: ArtifactSourceProperties
properties_list:
- description: The folder containing Azure Resource Manager templates.
  name: armTemplateFolderPath
  type: string
- description: The artifact source's branch reference.
  name: branchRef
  type: string
- description: The artifact source's creation date.
  name: createdDate
  type: string
- description: The artifact source's display name.
  name: displayName
  type: string
- description: The folder containing artifacts.
  name: folderPath
  type: string
- description: The provisioning status of the resource.
  name: provisioningState
  type: string
- description: The security token to authenticate to the artifact source.
  name: securityToken
  type: string
- description: The artifact source's type.
  name: sourceType
  type: string
- description: 'Indicates if the artifact source is enabled (values: Enabled, Disabled).'
  name: status
  type: string
- description: The unique immutable identifier of a resource (Guid).
  name: uniqueIdentifier
  type: string
- description: The artifact source's URI.
  name: uri
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-source-properties-schema.json
slug: azure-test-labs-artifact-source-properties
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactSourceProperties
---
