---
description: DeleteServiceSyncConfigInput schema from Amazon Proton API
layout: schema
name: DeleteServiceSyncConfigInput
properties_list:
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-service-sync-config-input-schema.json
slug: amazon-proton-delete-service-sync-config-input
source_filename: amazon-proton-delete-service-sync-config-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-service-sync-config-input-schema.json\",\n  \"title\": \"DeleteServiceSyncConfigInput\",\n  \"description\": \"DeleteServiceSyncConfigInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that you want to delete the service sync configuration for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-service-sync-config-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteServiceSyncConfigInput
---
