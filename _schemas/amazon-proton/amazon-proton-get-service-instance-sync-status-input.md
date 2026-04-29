---
description: GetServiceInstanceSyncStatusInput schema from Amazon Proton API
layout: schema
name: GetServiceInstanceSyncStatusInput
properties_list:
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-service-instance-sync-status-input-schema.json
slug: amazon-proton-get-service-instance-sync-status-input
source_filename: amazon-proton-get-service-instance-sync-status-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-instance-sync-status-input-schema.json\",\n  \"title\": \"GetServiceInstanceSyncStatusInput\",\n  \"description\": \"GetServiceInstanceSyncStatusInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service instance that you want the sync status input for.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that the service instance belongs to.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"serviceInstanceName\",\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-instance-sync-status-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetServiceInstanceSyncStatusInput
---
