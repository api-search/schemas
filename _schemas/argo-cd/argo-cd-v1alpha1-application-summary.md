---
description: v1alpha1ApplicationSummary schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSummary
properties_list:
- description: ExternalURLs holds all external URLs of application child resources.
  name: externalURLs
  type: array
- description: Images holds all images of application child resources.
  name: images
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-summary-schema.json
slug: argo-cd-v1alpha1-application-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-summary-schema.json\",\n  \"title\": \"v1alpha1ApplicationSummary\",\n  \"description\": \"v1alpha1ApplicationSummary schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalURLs\": {\n      \"description\": \"ExternalURLs holds all external URLs of application child resources.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"images\": {\n      \"description\": \"Images holds all images of application child resources.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-summary-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSummary
---
