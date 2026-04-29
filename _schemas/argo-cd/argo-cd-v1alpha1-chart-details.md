---
description: v1alpha1ChartDetails schema from Argo CD API
layout: schema
name: v1alpha1ChartDetails
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: home
  type: string
- description: ''
  name: maintainers
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-chart-details-schema.json
slug: argo-cd-v1alpha1-chart-details
source_filename: argo-cd-v1alpha1-chart-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-chart-details-schema.json\",\n  \"title\": \"v1alpha1ChartDetails\",\n  \"description\": \"v1alpha1ChartDetails schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"home\": {\n      \"type\": \"string\",\n      \"title\": \"The URL of this projects home page, e.g. \\\"http://example.com\\\"\"\n    },\n    \"maintainers\": {\n      \"type\": \"array\",\n      \"title\": \"List of maintainer details, name and email, e.g. [\\\"John Doe <john_doe@my-company.com>\\\"]\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-chart-details-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ChartDetails
---
