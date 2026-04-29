---
description: Properties of an artifact.
layout: schema
name: ArtifactInstallProperties
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
schema_file: json-schema/azure-test-labs-artifact-install-properties-schema.json
slug: azure-test-labs-artifact-install-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-install-properties-schema.json\",\n  \"title\": \"ArtifactInstallProperties\",\n  \"description\": \"Properties of an artifact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifactId\": {\n      \"description\": \"The artifact's identifier.\",\n      \"type\": \"string\"\n    },\n    \"artifactTitle\": {\n      \"description\": \"The artifact's title.\",\n      \"type\": \"string\"\n    },\n    \"deploymentStatusMessage\": {\n      \"description\": \"The status message from the deployment.\",\n      \"type\": \"string\"\n    },\n    \"installTime\": {\n      \"description\": \"The time that the artifact starts to install on the virtual machine.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"description\": \"\
  The parameters of the artifact.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ArtifactParameterProperties\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"description\": \"The status of the artifact.\",\n      \"type\": \"string\"\n    },\n    \"vmExtensionStatusMessage\": {\n      \"description\": \"The status message from the virtual machine extension.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-install-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactInstallProperties
---
