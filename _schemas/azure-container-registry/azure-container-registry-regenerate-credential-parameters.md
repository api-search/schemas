---
description: The parameters used to regenerate the login credential.
layout: schema
name: RegenerateCredentialParameters
properties_list:
- description: Specifies name of the password which should be regenerated -- password or password2.
  name: name
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-regenerate-credential-parameters-schema.json
slug: azure-container-registry-regenerate-credential-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-regenerate-credential-parameters-schema.json\",\n  \"title\": \"RegenerateCredentialParameters\",\n  \"description\": \"The parameters used to regenerate the login credential.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Specifies name of the password which should be regenerated -- password or password2.\",\n      \"enum\": [\n        \"password\",\n        \"password2\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"PasswordName\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-regenerate-credential-parameters-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: RegenerateCredentialParameters
---
