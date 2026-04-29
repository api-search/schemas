---
description: projectDetailedProjectsResponse schema from Argo CD API
layout: schema
name: projectDetailedProjectsResponse
properties_list:
- description: ''
  name: clusters
  type: array
- description: ''
  name: globalProjects
  type: array
- description: ''
  name: project
  type: object
- description: ''
  name: repositories
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-project-detailed-projects-response-schema.json
slug: argo-cd-project-detailed-projects-response
source_filename: argo-cd-project-detailed-projects-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-detailed-projects-response-schema.json\",\n  \"title\": \"projectDetailedProjectsResponse\",\n  \"description\": \"projectDetailedProjectsResponse schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Cluster\"\n      }\n    },\n    \"globalProjects\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1AppProject\"\n      }\n    },\n    \"project\": {\n      \"$ref\": \"#/definitions/v1alpha1AppProject\"\n    },\n    \"repositories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Repository\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-project-detailed-projects-response-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: projectDetailedProjectsResponse
---
