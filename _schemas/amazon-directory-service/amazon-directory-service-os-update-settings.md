---
description: OS version that the directory needs to be updated to.
layout: schema
name: OSUpdateSettings
properties_list:
- description: ''
  name: OSVersion
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-os-update-settings-schema.json
slug: amazon-directory-service-os-update-settings
source_filename: amazon-directory-service-os-update-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-os-update-settings-schema.json\",\n  \"title\": \"OSUpdateSettings\",\n  \"description\": \" OS version that the directory needs to be updated to. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OSVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OSVersion\"\n        },\n        {\n          \"description\": \" OS version that the directory needs to be updated to. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-os-update-settings-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: OSUpdateSettings
---
