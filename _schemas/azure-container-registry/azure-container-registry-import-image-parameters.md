---
description: ImportImageParameters schema from Azure Container Registry API
layout: schema
name: ImportImageParameters
properties_list:
- description: When Force, any existing target tags will be overwritten. When NoForce, any existing target tags will fail the operation before any copying begins.
  name: mode
  type: string
- description: The source of the image.
  name: source
  type: object
- description: List of strings of the form repo[:tag]. When tag is omitted the source will be used (or 'latest' if source tag is also omitted).
  name: targetTags
  type: array
- description: List of strings of repository names to do a manifest only copy. No tag will be created.
  name: untaggedTargetRepositories
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-import-image-parameters-schema.json
slug: azure-container-registry-import-image-parameters
source_filename: azure-container-registry-import-image-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-import-image-parameters-schema.json\",\n  \"title\": \"ImportImageParameters\",\n  \"description\": \"ImportImageParameters schema from Azure Container Registry API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mode\": {\n      \"default\": \"NoForce\",\n      \"description\": \"When Force, any existing target tags will be overwritten. When NoForce, any existing target tags will fail the operation before any copying begins.\",\n      \"enum\": [\n        \"NoForce\",\n        \"Force\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ImportMode\"\n      }\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/ImportSource\",\n      \"description\": \"The source of the image.\"\n    },\n\
  \    \"targetTags\": {\n      \"description\": \"List of strings of the form repo[:tag]. When tag is omitted the source will be used (or 'latest' if source tag is also omitted).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"untaggedTargetRepositories\": {\n      \"description\": \"List of strings of repository names to do a manifest only copy. No tag will be created.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-import-image-parameters-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: ImportImageParameters
---
