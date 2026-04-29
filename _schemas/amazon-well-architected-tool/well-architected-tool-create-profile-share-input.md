---
description: CreateProfileShareInput schema from AWS Well-Architected Tool API
layout: schema
name: CreateProfileShareInput
properties_list:
- description: ''
  name: SharedWith
  type: object
- description: ''
  name: ClientRequestToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-profile-share-input-schema.json
slug: well-architected-tool-create-profile-share-input
source_filename: well-architected-tool-create-profile-share-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"SharedWith\",\n    \"ClientRequestToken\"\n  ],\n  \"title\": \"CreateProfileShareInput\",\n  \"properties\": {\n    \"SharedWith\": {\n      \"$ref\": \"#/components/schemas/SharedWith\"\n    },\n    \"ClientRequestToken\": {\n      \"$ref\": \"#/components/schemas/ClientRequestToken\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-share-input-schema.json\",\n  \"description\": \"CreateProfileShareInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-share-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateProfileShareInput
---
