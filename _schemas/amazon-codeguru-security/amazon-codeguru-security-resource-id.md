---
description: The identifier for a resource object that contains resources where a finding was detected.
layout: schema
name: ResourceId
properties_list:
- description: ''
  name: codeArtifactId
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-resource-id-schema.json
slug: amazon-codeguru-security-resource-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-resource-id-schema.json\",\n  \"title\": \"ResourceId\",\n  \"description\": \"The identifier for a resource object that contains resources where a finding was detected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeArtifactId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The identifier for the code file uploaded to the resource where a finding was detected.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-resource-id-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: ResourceId
---
