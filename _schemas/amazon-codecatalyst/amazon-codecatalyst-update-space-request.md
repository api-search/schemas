---
description: UpdateSpaceRequest schema from Amazon CodeCatalyst
layout: schema
name: UpdateSpaceRequest
properties_list:
- description: ''
  name: description
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-update-space-request-schema.json
slug: amazon-codecatalyst-update-space-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-space-request-schema.json\",\n  \"title\": \"UpdateSpaceRequest\",\n  \"description\": \"UpdateSpaceRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpaceDescription\"\n        },\n        {\n          \"description\": \"The description of the space.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-update-space-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: UpdateSpaceRequest
---
