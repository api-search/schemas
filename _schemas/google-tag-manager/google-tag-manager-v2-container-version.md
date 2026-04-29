---
description: Represents a version of a Google Tag Manager Container. A container version is a snapshot of all tags, triggers, variables, and configuration at a point in time.
layout: schema
name: ContainerVersion
properties_list:
- description: GTM ContainerVersion's API relative path.
  name: path
  type: string
- description: GTM Account ID.
  name: accountId
  type: string
- description: GTM Container ID.
  name: containerId
  type: string
- description: The Container Version ID uniquely identifies the GTM Container Version.
  name: containerVersionId
  type: string
- description: Container version display name.
  name: name
  type: string
- description: Container version description.
  name: description
  type: string
- description: The tags in the container that this version was taken from.
  name: tag
  type: array
- description: The triggers in the container that this version was taken from.
  name: trigger
  type: array
- description: The variables in the container that this version was taken from.
  name: variable
  type: array
- description: The fingerprint of the GTM Container Version as computed at storage time.
  name: fingerprint
  type: string
- description: Auto-generated link to the tag manager UI.
  name: tagManagerUrl
  type: string
- description: A value of true indicates this version has been deleted.
  name: deleted
  type: boolean
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-container-version-schema.json
slug: google-tag-manager-v2-container-version
source_filename: google-tag-manager-v2-container-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerVersion\",\n  \"type\": \"object\",\n  \"description\": \"Represents a version of a Google Tag Manager Container. A container version is a snapshot of all tags, triggers, variables, and configuration at a point in time.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"GTM ContainerVersion's API relative path.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Account ID.\"\n    },\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Container ID.\"\n    },\n    \"containerVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"The Container Version ID uniquely identifies the GTM Container Version.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Container version display name.\"\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Container version description.\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"description\": \"The tags in the container that this version was taken from.\"\n    },\n    \"trigger\": {\n      \"type\": \"array\",\n      \"description\": \"The triggers in the container that this version was taken from.\"\n    },\n    \"variable\": {\n      \"type\": \"array\",\n      \"description\": \"The variables in the container that this version was taken from.\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The fingerprint of the GTM Container Version as computed at storage time.\"\n    },\n    \"tagManagerUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated link to the tag manager UI.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"A value of true indicates this version has been deleted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-container-version-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: ContainerVersion
---
