---
description: Properties of an artifact deployment.
layout: schema
name: ArtifactDeploymentStatusProperties
properties_list:
- description: The total count of the artifacts that were successfully applied.
  name: artifactsApplied
  type: integer
- description: The deployment status of the artifact.
  name: deploymentStatus
  type: string
- description: The total count of the artifacts that were tentatively applied.
  name: totalArtifacts
  type: integer
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-deployment-status-properties-schema.json
slug: azure-test-labs-artifact-deployment-status-properties
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactDeploymentStatusProperties
---
