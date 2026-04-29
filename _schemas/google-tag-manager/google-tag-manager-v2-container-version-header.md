---
description: Represents a summary of a container version, without the full tag, trigger, and variable details.
layout: schema
name: ContainerVersionHeader
properties_list:
- description: GTM Container Version's API relative path.
  name: path
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: containerId
  type: string
- description: ''
  name: containerVersionId
  type: string
- description: Container version display name.
  name: name
  type: string
- description: Number of tags in the container version.
  name: numTags
  type: string
- description: Number of triggers in the container version.
  name: numTriggers
  type: string
- description: Number of variables in the container version.
  name: numVariables
  type: string
- description: ''
  name: deleted
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-container-version-header-schema.json
slug: google-tag-manager-v2-container-version-header
source_filename: google-tag-manager-v2-container-version-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerVersionHeader\",\n  \"type\": \"object\",\n  \"description\": \"Represents a summary of a container version, without the full tag, trigger, and variable details.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Container Version's API relative path.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"containerId\": {\n      \"type\": \"string\"\n    },\n    \"containerVersionId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Container version display name.\"\n    },\n    \"numTags\": {\n      \"type\": \"string\",\n      \"description\": \"Number of tags in the container version.\"\n    },\n    \"numTriggers\": {\n      \"type\": \"string\",\n      \"description\": \"Number of triggers in the container version.\"\n    },\n    \"numVariables\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Number of variables in the container version.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-container-version-header-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ContainerVersionHeader
---
