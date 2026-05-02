---
description: A permission assignment in an Intralinks workspace that controls group-level access to folders and documents. Permissions determine whether content is visible to participant groups.
layout: schema
name: Intralinks Permission
properties_list:
- description: Unique identifier of the permission.
  name: id
  type: string
- description: ID of the group this permission is assigned to.
  name: groupId
  type: string
- description: ID of the folder this permission applies to.
  name: folderId
  type: string
- description: Permission level granted to the group.
  name: permission
  type: string
provider_name: Intralinks
provider_slug: intralinks
schema_file: json-schema/permission.json
slug: permission
source_filename: permission.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"permission.json\",\n  \"title\": \"Intralinks Permission\",\n  \"description\": \"A permission assignment in an Intralinks workspace that controls group-level access to folders and documents. Permissions determine whether content is visible to participant groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the permission.\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the group this permission is assigned to.\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the folder this permission applies to.\"\n    },\n    \"permission\": {\n      \"type\": \"string\",\n      \"enum\": [\"SEE\", \"SEE_AND_DOWNLOAD\", \"SEE_DOWNLOAD_AND_PRINT\"],\n      \"description\": \"Permission level granted to the group.\"\n    }\n  },\n\
  \  \"required\": [\"groupId\", \"folderId\", \"permission\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/json-schema/permission.json
tags:
- Document Management
- Secure File Sharing
- Virtual Data Room
title: Intralinks Permission
---
