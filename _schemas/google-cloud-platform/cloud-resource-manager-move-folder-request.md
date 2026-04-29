---
description: Request message for moving a folder.
layout: schema
name: MoveFolderRequest
properties_list:
- description: The resource name of the folder or organization which should be the new parent of the folder.
  name: destinationParent
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-move-folder-request-schema.json
slug: cloud-resource-manager-move-folder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MoveFolderRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request message for moving a folder.\",\n  \"properties\": {\n    \"destinationParent\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the folder or organization which should be the new parent of the folder.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-move-folder-request-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: MoveFolderRequest
---
