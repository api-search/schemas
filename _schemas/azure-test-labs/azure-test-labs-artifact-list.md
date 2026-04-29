---
description: The response of a list operation.
layout: schema
name: ArtifactList
properties_list:
- description: Link for next set of results.
  name: nextLink
  type: string
- description: Results of the list operation.
  name: value
  type: array
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-list-schema.json
slug: azure-test-labs-artifact-list
source_filename: azure-test-labs-artifact-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-list-schema.json\",\n  \"title\": \"ArtifactList\",\n  \"description\": \"The response of a list operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"Link for next set of results.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Results of the list operation.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Artifact\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-list-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ArtifactList
---
