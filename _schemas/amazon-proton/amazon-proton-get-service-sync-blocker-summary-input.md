---
description: GetServiceSyncBlockerSummaryInput schema from Amazon Proton API
layout: schema
name: GetServiceSyncBlockerSummaryInput
properties_list:
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-service-sync-blocker-summary-input-schema.json
slug: amazon-proton-get-service-sync-blocker-summary-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-sync-blocker-summary-input-schema.json\",\n  \"title\": \"GetServiceSyncBlockerSummaryInput\",\n  \"description\": \"GetServiceSyncBlockerSummaryInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service instance that you want to get the service sync blocker summary for. If given bothe the instance name and the service name, only the instance is blocked.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of\
  \ the service that you want to get the service sync blocker summary for. If given only the service name, all instances are blocked.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-sync-blocker-summary-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetServiceSyncBlockerSummaryInput
---
