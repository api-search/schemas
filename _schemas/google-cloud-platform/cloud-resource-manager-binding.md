---
description: Associates members with a role.
layout: schema
name: Binding
properties_list:
- description: 'The role that is assigned to the list of members. Example: roles/resourcemanager.projectViewer.'
  name: role
  type: string
- description: The identities requesting access. Supports user, serviceAccount, group, and domain members.
  name: members
  type: array
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-binding-schema.json
slug: cloud-resource-manager-binding
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Binding\",\n  \"type\": \"object\",\n  \"description\": \"Associates members with a role.\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role that is assigned to the list of members. Example: roles/resourcemanager.projectViewer.\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"The identities requesting access. Supports user, serviceAccount, group, and domain members.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-binding-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: Binding
---
