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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-deployment-status-properties-schema.json\",\n  \"title\": \"ArtifactDeploymentStatusProperties\",\n  \"description\": \"Properties of an artifact deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifactsApplied\": {\n      \"description\": \"The total count of the artifacts that were successfully applied.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"deploymentStatus\": {\n      \"description\": \"The deployment status of the artifact.\",\n      \"type\": \"string\"\n    },\n    \"totalArtifacts\": {\n      \"description\": \"The total count of the artifacts that were tentatively applied.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-deployment-status-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactDeploymentStatusProperties
---
