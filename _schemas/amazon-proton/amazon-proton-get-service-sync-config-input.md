---
description: GetServiceSyncConfigInput schema from Amazon Proton API
layout: schema
name: GetServiceSyncConfigInput
properties_list:
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-service-sync-config-input-schema.json
slug: amazon-proton-get-service-sync-config-input
source_filename: amazon-proton-get-service-sync-config-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-sync-config-input-schema.json\",\n  \"title\": \"GetServiceSyncConfigInput\",\n  \"description\": \"GetServiceSyncConfigInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that you want to get the service sync configuration for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-sync-config-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetServiceSyncConfigInput
---
