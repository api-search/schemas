---
description: Properties of an artifact.
layout: schema
name: ArtifactProperties
properties_list:
- description: The artifact's creation date.
  name: createdDate
  type: string
- description: The artifact's description.
  name: description
  type: string
- description: The file path to the artifact.
  name: filePath
  type: string
- description: The URI to the artifact icon.
  name: icon
  type: string
- description: The artifact's parameters.
  name: parameters
  type: object
- description: The artifact's publisher.
  name: publisher
  type: string
- description: The artifact's target OS.
  name: targetOsType
  type: string
- description: The artifact's title.
  name: title
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-properties-schema.json
slug: azure-test-labs-artifact-properties
source_filename: azure-test-labs-artifact-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-properties-schema.json\",\n  \"title\": \"ArtifactProperties\",\n  \"description\": \"Properties of an artifact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdDate\": {\n      \"description\": \"The artifact's creation date.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"The artifact's description.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"filePath\": {\n      \"description\": \"The file path to the artifact.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"icon\": {\n      \"description\": \"The URI to the artifact icon.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"parameters\"\
  : {\n      \"description\": \"The artifact's parameters.\",\n      \"readOnly\": true,\n      \"type\": \"object\"\n    },\n    \"publisher\": {\n      \"description\": \"The artifact's publisher.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"targetOsType\": {\n      \"description\": \"The artifact's target OS.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"description\": \"The artifact's title.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactProperties
---
