---
description: Properties of an artifact parameter.
layout: schema
name: ArtifactParameterProperties
properties_list:
- description: The name of the artifact parameter.
  name: name
  type: string
- description: The value of the artifact parameter.
  name: value
  type: string
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-parameter-properties-schema.json
slug: azure-test-labs-artifact-parameter-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-parameter-properties-schema.json\",\n  \"title\": \"ArtifactParameterProperties\",\n  \"description\": \"Properties of an artifact parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the artifact parameter.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The value of the artifact parameter.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-parameter-properties-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactParameterProperties
---
