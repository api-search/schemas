---
description: GetRepositorySyncStatusOutput schema from Amazon Proton API
layout: schema
name: GetRepositorySyncStatusOutput
properties_list:
- description: ''
  name: latestSync
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-repository-sync-status-output-schema.json
slug: amazon-proton-get-repository-sync-status-output
source_filename: amazon-proton-get-repository-sync-status-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-repository-sync-status-output-schema.json\",\n  \"title\": \"GetRepositorySyncStatusOutput\",\n  \"description\": \"GetRepositorySyncStatusOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latestSync\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositorySyncAttempt\"\n        },\n        {\n          \"description\": \"The repository sync status detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-repository-sync-status-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetRepositorySyncStatusOutput
---
