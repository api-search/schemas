---
description: A tag key, used to group tag values. Tag keys define namespaces for tag values that can be attached to resources for organization and policy purposes.
layout: schema
name: TagKey
properties_list:
- description: The resource name of the tag key in the form tagKeys/{tag_key_id}. Output only.
  name: name
  type: string
- description: The resource name of the parent. Must be of the form organizations/{org_id}.
  name: parent
  type: string
- description: The user-friendly short name for the tag key. The short name must be unique within the same parent and have a maximum length of 256 characters.
  name: shortName
  type: string
- description: The namespaced name of the tag key in the form {parentId}/{shortName}. Output only.
  name: namespacedName
  type: string
- description: User-assigned description of the tag key. Maximum length of 256 characters.
  name: description
  type: string
- description: Timestamp when the tag key was created. Output only.
  name: createTime
  type: string
- description: Timestamp when the tag key was last modified. Output only.
  name: updateTime
  type: string
- description: Entity tag for optimistic concurrency control.
  name: etag
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-tag-key-schema.json
slug: cloud-resource-manager-tag-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagKey\",\n  \"type\": \"object\",\n  \"description\": \"A tag key, used to group tag values. Tag keys define namespaces for tag values that can be attached to resources for organization and policy purposes.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the tag key in the form tagKeys/{tag_key_id}. Output only.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the parent. Must be of the form organizations/{org_id}.\"\n    },\n    \"shortName\": {\n      \"type\": \"string\",\n      \"description\": \"The user-friendly short name for the tag key. The short name must be unique within the same parent and have a maximum length of 256 characters.\"\n    },\n    \"namespacedName\": {\n      \"type\": \"string\",\n      \"description\": \"The namespaced name of the tag key in\
  \ the form {parentId}/{shortName}. Output only.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-assigned description of the tag key. Maximum length of 256 characters.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the tag key was created. Output only.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the tag key was last modified. Output only.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag for optimistic concurrency control.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-tag-key-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: TagKey
---
