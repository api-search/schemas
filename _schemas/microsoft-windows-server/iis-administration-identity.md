---
description: The identity configuration for the application pool worker process.
layout: schema
name: Identity
properties_list:
- description: The type of identity used by the application pool.
  name: identity_type
  type: string
- description: The username for the identity when using SpecificUser identity type.
  name: username
  type: string
- description: Whether to load the user profile for the worker process.
  name: load_user_profile
  type: boolean
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-identity-schema.json
slug: iis-administration-identity
source_filename: iis-administration-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Identity\",\n  \"type\": \"object\",\n  \"description\": \"The identity configuration for the application pool worker process.\",\n  \"properties\": {\n    \"identity_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity used by the application pool.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username for the identity when using SpecificUser identity type.\"\n    },\n    \"load_user_profile\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to load the user profile for the worker process.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-identity-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: Identity
---
