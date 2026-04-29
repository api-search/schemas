---
description: Request body for triggering a service deployment
layout: schema
name: DeployServiceRequest
properties_list:
- description: Version tag to deploy
  name: version
  type: string
- description: Container image with version tag
  name: image
  type: string
- description: Deployment strategy
  name: strategy
  type: string
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-deploy-service-request-schema.json
slug: platform-services-deploy-service-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-deploy-service-request-schema.json\",\n  \"title\": \"DeployServiceRequest\",\n  \"description\": \"Request body for triggering a service deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version tag to deploy\",\n      \"example\": \"2.6.0\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Container image with version tag\",\n      \"example\": \"allianz/policy-service:2.6.0\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment strategy\",\n      \"enum\": [\n        \"rolling\",\n        \"blue_green\",\n        \"canary\"\n      ],\n      \"default\": \"rolling\",\n      \"example\": \"rolling\"\n    }\n  },\n\
  \  \"required\": [\n    \"version\",\n    \"image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-deploy-service-request-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: DeployServiceRequest
---
