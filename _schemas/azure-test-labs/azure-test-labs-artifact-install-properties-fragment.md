---
description: Properties of an artifact.
layout: schema
name: ArtifactInstallPropertiesFragment
properties_list:
- description: The artifact's identifier.
  name: artifactId
  type: string
- description: The artifact's title.
  name: artifactTitle
  type: string
- description: The status message from the deployment.
  name: deploymentStatusMessage
  type: string
- description: The time that the artifact starts to install on the virtual machine.
  name: installTime
  type: string
- description: The parameters of the artifact.
  name: parameters
  type: array
- description: The status of the artifact.
  name: status
  type: string
- description: The status message from the virtual machine extension.
  name: vmExtensionStatusMessage
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-install-properties-fragment-schema.json
slug: azure-test-labs-artifact-install-properties-fragment
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactInstallPropertiesFragment
---
