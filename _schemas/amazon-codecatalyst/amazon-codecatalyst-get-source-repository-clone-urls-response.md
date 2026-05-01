---
description: GetSourceRepositoryCloneUrlsResponse schema from Amazon CodeCatalyst
layout: schema
name: GetSourceRepositoryCloneUrlsResponse
properties_list:
- description: ''
  name: https
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-get-source-repository-clone-urls-response-schema.json
slug: amazon-codecatalyst-get-source-repository-clone-urls-response
source_filename: amazon-codecatalyst-get-source-repository-clone-urls-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-source-repository-clone-urls-response-schema.json\",\n  \"title\": \"GetSourceRepositoryCloneUrlsResponse\",\n  \"description\": \"GetSourceRepositoryCloneUrlsResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"https\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The HTTPS URL to use when cloning the source repository.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"https\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-source-repository-clone-urls-response-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: GetSourceRepositoryCloneUrlsResponse
---
