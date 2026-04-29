---
description: Request body for applying artifacts to a virtual machine.
layout: schema
name: ApplyArtifactsRequest
properties_list:
- description: The list of artifacts to apply.
  name: artifacts
  type: array
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schema_file: json-schema/azure-test-labs-apply-artifacts-request-schema.json
slug: azure-test-labs-apply-artifacts-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-apply-artifacts-request-schema.json\",\n  \"title\": \"ApplyArtifactsRequest\",\n  \"description\": \"Request body for applying artifacts to a virtual machine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"artifacts\": {\n      \"description\": \"The list of artifacts to apply.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ArtifactInstallProperties\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/json-schema/azure-test-labs-apply-artifacts-request-schema.json
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
title: ApplyArtifactsRequest
---
