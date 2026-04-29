---
description: The ImmutabilityPolicy property of a blob container, including Id, resource name, resource type, Etag.
layout: schema
name: ImmutabilityPolicy
properties_list:
- description: The properties of an ImmutabilityPolicy of a blob container.
  name: properties
  type: object
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-immutability-policy-schema.json
slug: azure-storage-account-immutability-policy
source_filename: azure-storage-account-immutability-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-immutability-policy-schema.json\",\n  \"title\": \"ImmutabilityPolicy\",\n  \"description\": \"The ImmutabilityPolicy property of a blob container, including Id, resource name, resource type, Etag.\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ImmutabilityPolicyProperty\",\n      \"description\": \"The properties of an ImmutabilityPolicy of a blob container.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-immutability-policy-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ImmutabilityPolicy
---
