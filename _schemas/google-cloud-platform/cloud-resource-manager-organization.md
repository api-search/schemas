---
description: The root node in the resource hierarchy to which a particular entity's resources belong. An organization is tied to a Google Workspace or Cloud Identity account. Organizations cannot be created or deleted through the API; they are automatically provisioned when a Google Workspace or Cloud Identity account is created.
layout: schema
name: Organization
properties_list:
- description: The resource name of the organization in the form organizations/{organization_id}. Output only.
  name: name
  type: string
- description: A human-readable string that refers to the organization in the Google Cloud Console. This field is output only and derived from the associated Google Workspace or Cloud Identity account.
  name: displayName
  type: string
- description: The unique identifier for the Google Workspace or Cloud Identity account associated with this organization. Output only.
  name: directoryCustomerId
  type: string
- description: The organization lifecycle state. Output only.
  name: state
  type: string
- description: Timestamp when the organization was created. Output only.
  name: createTime
  type: string
- description: Timestamp when the organization was last modified. Output only.
  name: updateTime
  type: string
- description: Timestamp of when the delete request was sent. Output only.
  name: deleteTime
  type: string
- description: A checksum computed by the server based on the current value of the organization resource.
  name: etag
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-organization-schema.json
slug: cloud-resource-manager-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"description\": \"The root node in the resource hierarchy to which a particular entity's resources belong. An organization is tied to a Google Workspace or Cloud Identity account. Organizations cannot be created or deleted through the API; they are automatically provisioned when a Google Workspace or Cloud Identity account is created.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the organization in the form organizations/{organization_id}. Output only.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable string that refers to the organization in the Google Cloud Console. This field is output only and derived from the associated Google Workspace or Cloud Identity account.\"\n    },\n    \"directoryCustomerId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The unique identifier for the Google Workspace or Cloud Identity account associated with this organization. Output only.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The organization lifecycle state. Output only.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the organization was created. Output only.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the organization was last modified. Output only.\"\n    },\n    \"deleteTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the delete request was sent. Output only.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"A checksum computed by the server based on the current value of the organization resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-organization-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: Organization
---
