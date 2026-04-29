---
description: A service deployment record on the platform
layout: schema
name: Deployment
properties_list:
- description: Unique identifier for the deployment
  name: deployment_id
  type: string
- description: Service this deployment belongs to
  name: service_id
  type: string
- description: Version being deployed
  name: version
  type: string
- description: Container image with tag
  name: image
  type: string
- description: Current deployment status
  name: status
  type: string
- description: Deployment strategy used
  name: strategy
  type: string
- description: Timestamp when the deployment completed
  name: deployed_at
  type: string
- description: Actor that triggered the deployment
  name: deployed_by
  type: string
- description: Timestamp when the deployment was initiated
  name: initiated_at
  type: string
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-deployment-schema.json
slug: platform-services-deployment
source_filename: platform-services-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-deployment-schema.json\",\n  \"title\": \"Deployment\",\n  \"description\": \"A service deployment record on the platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the deployment\",\n      \"example\": \"dep-500789\"\n    },\n    \"service_id\": {\n      \"type\": \"string\",\n      \"description\": \"Service this deployment belongs to\",\n      \"example\": \"svc-500123\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version being deployed\",\n      \"example\": \"2.5.1\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Container image with tag\",\n      \"example\": \"allianz/policy-service:2.5.1\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current deployment status\",\n      \"enum\": [\n        \"in_progress\",\n        \"succeeded\",\n        \"failed\",\n        \"rolled_back\"\n      ],\n      \"example\": \"succeeded\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment strategy used\",\n      \"enum\": [\n        \"rolling\",\n        \"blue_green\",\n        \"canary\"\n      ],\n      \"example\": \"rolling\"\n    },\n    \"deployed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment completed\",\n      \"example\": \"2026-04-15T14:30:00Z\"\n    },\n    \"deployed_by\": {\n      \"type\": \"string\",\n      \"description\": \"Actor that triggered the deployment\",\n      \"example\": \"argo-cd\"\n    },\n    \"initiated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  Timestamp when the deployment was initiated\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-deployment-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: Deployment
---
