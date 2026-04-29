---
description: An artifact.
layout: schema
name: Artifact
properties_list:
- description: The properties of the resource.
  name: properties
  type: object
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-artifact-schema.json
slug: azure-test-labs-artifact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-schema.json\",\n  \"title\": \"Artifact\",\n  \"description\": \"An artifact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ArtifactProperties\",\n      \"description\": \"The properties of the resource.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-artifact-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: Artifact
---
