---
description: A folder in the Google Cloud resource hierarchy. Folders can contain projects and other folders, allowing users to group resources and apply policies hierarchically. Folders can be up to 10 levels deep.
layout: schema
name: Folder
properties_list:
- description: The resource name of the folder in the form folders/{folder_id}. Output only.
  name: name
  type: string
- description: The resource name of the folder's parent. Can be an organization or another folder in the form organizations/{org_id} or folders/{folder_id}.
  name: parent
  type: string
- description: The folder's display name. A folder's display name must be distinct from all other folders that share its parent. The display name must start and end with a letter or digit, may contain letters, digit
  name: displayName
  type: string
- description: The lifecycle state of the folder. Output only.
  name: state
  type: string
- description: Timestamp of when the folder was created. Output only.
  name: createTime
  type: string
- description: Timestamp of when the folder was last modified. Output only.
  name: updateTime
  type: string
- description: Timestamp of when the delete request was sent. Output only.
  name: deleteTime
  type: string
- description: A checksum computed by the server based on the current value of the folder resource.
  name: etag
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-folder-schema.json
slug: cloud-resource-manager-folder
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Folder\",\n  \"type\": \"object\",\n  \"description\": \"A folder in the Google Cloud resource hierarchy. Folders can contain projects and other folders, allowing users to group resources and apply policies hierarchically. Folders can be up to 10 levels deep.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the folder in the form folders/{folder_id}. Output only.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the folder's parent. Can be an organization or another folder in the form organizations/{org_id} or folders/{folder_id}.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The folder's display name. A folder's display name must be distinct from all other folders that share its parent. The display name must start and end with\
  \ a letter or digit, may contain letters, digits, spaces, hyphens and underscores, and can be no longer than 30 characters.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state of the folder. Output only.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the folder was created. Output only.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the folder was last modified. Output only.\"\n    },\n    \"deleteTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the delete request was sent. Output only.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"A checksum computed by the server based on the current value of the folder resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-folder-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: Folder
---
