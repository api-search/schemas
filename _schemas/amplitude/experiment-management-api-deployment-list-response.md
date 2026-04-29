---
description: DeploymentListResponse schema from Amplitude Experiment Management API
layout: schema
name: DeploymentListResponse
properties_list:
- description: Array of deployment objects.
  name: deployments
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-management-api-deployment-list-response-schema.json
slug: experiment-management-api-deployment-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-deployment-list-response-schema.json\",\n  \"title\": \"DeploymentListResponse\",\n  \"description\": \"DeploymentListResponse schema from Amplitude Experiment Management API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployments\": {\n      \"type\": \"array\",\n      \"description\": \"Array of deployment objects.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the deployment.\"\n          },\n          \"projectId\": {\n            \"type\": \"string\",\n            \"description\": \"The project the deployment belongs to.\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The display label for the deployment.\"\n          },\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The deployment key used for API authentication.\"\n          },\n          \"deleted\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the deployment has been deleted.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-management-api-deployment-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: DeploymentListResponse
---
