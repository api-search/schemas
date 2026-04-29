---
description: A tag value, which is a child of a tag key. Tag values are the specific labels that can be attached to resources through tag bindings.
layout: schema
name: TagValue
properties_list:
- description: The resource name of the tag value in the form tagValues/{tag_value_id}. Output only.
  name: name
  type: string
- description: The resource name of the parent tag key.
  name: parent
  type: string
- description: The user-friendly short name for the tag value. Unique for a given tag key. Maximum length of 256 characters.
  name: shortName
  type: string
- description: The namespaced name of the tag value in the form {parentNamespace}/{shortName}. Output only.
  name: namespacedName
  type: string
- description: User-assigned description of the tag value. Maximum length of 256 characters.
  name: description
  type: string
- description: Timestamp when the tag value was created. Output only.
  name: createTime
  type: string
- description: Timestamp when the tag value was last modified. Output only.
  name: updateTime
  type: string
- description: Entity tag for optimistic concurrency control.
  name: etag
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-tag-value-schema.json
slug: cloud-resource-manager-tag-value
source_filename: cloud-resource-manager-tag-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagValue\",\n  \"type\": \"object\",\n  \"description\": \"A tag value, which is a child of a tag key. Tag values are the specific labels that can be attached to resources through tag bindings.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the tag value in the form tagValues/{tag_value_id}. Output only.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the parent tag key.\"\n    },\n    \"shortName\": {\n      \"type\": \"string\",\n      \"description\": \"The user-friendly short name for the tag value. Unique for a given tag key. Maximum length of 256 characters.\"\n    },\n    \"namespacedName\": {\n      \"type\": \"string\",\n      \"description\": \"The namespaced name of the tag value in the form {parentNamespace}/{shortName}. Output only.\"\n    },\n    \"description\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"User-assigned description of the tag value. Maximum length of 256 characters.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the tag value was created. Output only.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the tag value was last modified. Output only.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag for optimistic concurrency control.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-tag-value-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: TagValue
---
