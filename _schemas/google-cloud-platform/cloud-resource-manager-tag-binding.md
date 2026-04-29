---
description: A tag binding associates a tag value with a Google Cloud resource. Tag bindings represent the link between organization taxonomy (tag keys and values) and actual cloud resources.
layout: schema
name: TagBinding
properties_list:
- description: The resource name of the tag binding in the form tagBindings/{tag_binding_id}. Output only.
  name: name
  type: string
- description: 'The full resource name of the resource the tag value is bound to. Example: //cloudresourcemanager.googleapis.com/projects/123.'
  name: parent
  type: string
- description: The resource name of the tag value in the form tagValues/{tag_value_id}.
  name: tagValue
  type: string
- description: The namespaced name of the tag value in the form {parentNamespace}/{tagKeyShortName}/{tagValueShortName}. Output only.
  name: tagValueNamespacedName
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-tag-binding-schema.json
slug: cloud-resource-manager-tag-binding
source_filename: cloud-resource-manager-tag-binding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagBinding\",\n  \"type\": \"object\",\n  \"description\": \"A tag binding associates a tag value with a Google Cloud resource. Tag bindings represent the link between organization taxonomy (tag keys and values) and actual cloud resources.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the tag binding in the form tagBindings/{tag_binding_id}. Output only.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The full resource name of the resource the tag value is bound to. Example: //cloudresourcemanager.googleapis.com/projects/123.\"\n    },\n    \"tagValue\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the tag value in the form tagValues/{tag_value_id}.\"\n    },\n    \"tagValueNamespacedName\": {\n      \"type\": \"string\",\n      \"description\": \"The namespaced\
  \ name of the tag value in the form {parentNamespace}/{tagKeyShortName}/{tagValueShortName}. Output only.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-tag-binding-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: TagBinding
---
