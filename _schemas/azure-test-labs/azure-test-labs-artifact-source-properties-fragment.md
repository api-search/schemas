---
description: Properties of an artifact source.
layout: schema
name: ArtifactSourcePropertiesFragment
properties_list:
- description: The folder containing Azure Resource Manager templates.
  name: armTemplateFolderPath
  type: string
- description: The artifact source's branch reference.
  name: branchRef
  type: string
- description: The artifact source's display name.
  name: displayName
  type: string
- description: The folder containing artifacts.
  name: folderPath
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
- description: The artifact source's URI.
  name: uri
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-source-properties-fragment-schema.json
slug: azure-test-labs-artifact-source-properties-fragment
source_filename: azure-test-labs-artifact-source-properties-fragment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-source-properties-fragment-schema.json\",\n  \"title\": \"ArtifactSourcePropertiesFragment\",\n  \"description\": \"Properties of an artifact source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"armTemplateFolderPath\": {\n      \"description\": \"The folder containing Azure Resource Manager templates.\",\n      \"type\": \"string\"\n    },\n    \"branchRef\": {\n      \"description\": \"The artifact source's branch reference.\",\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"The artifact source's display name.\",\n      \"type\": \"string\"\n    },\n    \"folderPath\": {\n      \"description\": \"The folder containing artifacts.\",\n      \"type\": \"string\"\n    },\n    \"securityToken\": {\n      \"description\": \"The security\
  \ token to authenticate to the artifact source.\",\n      \"type\": \"string\"\n    },\n    \"sourceType\": {\n      \"description\": \"The artifact source's type.\",\n      \"enum\": [\n        \"VsoGit\",\n        \"GitHub\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"SourceControlType\"\n      }\n    },\n    \"status\": {\n      \"description\": \"Indicates if the artifact source is enabled (values: Enabled, Disabled).\",\n      \"enum\": [\n        \"Enabled\",\n        \"Disabled\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"EnableStatus\"\n      }\n    },\n    \"uri\": {\n      \"description\": \"The artifact source's URI.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-source-properties-fragment-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactSourcePropertiesFragment
---
