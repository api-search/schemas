---
description: Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.
layout: schema
name: DirectoryObject
properties_list:
- description: The OData type of the directory object.
  name: '@odata.type'
  type: string
- description: The unique identifier for the directory object.
  name: id
  type: string
- description: The name displayed for the directory object.
  name: displayName
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-directory-object-schema.json
slug: microsoft-graph-directory-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DirectoryObject\",\n  \"type\": \"object\",\n  \"description\": \"Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"description\": \"The OData type of the directory object.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the directory object.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed for the directory object.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-directory-object-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: DirectoryObject
---
