---
description: v1alpha1SuccessfulHydrateOperation schema from Argo CD API
layout: schema
name: v1alpha1SuccessfulHydrateOperation
properties_list:
- description: ''
  name: drySHA
  type: string
- description: ''
  name: hydratedSHA
  type: string
- description: ''
  name: sourceHydrator
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-successful-hydrate-operation-schema.json
slug: argo-cd-v1alpha1-successful-hydrate-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-successful-hydrate-operation-schema.json\",\n  \"title\": \"v1alpha1SuccessfulHydrateOperation\",\n  \"description\": \"v1alpha1SuccessfulHydrateOperation schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"drySHA\": {\n      \"type\": \"string\",\n      \"title\": \"DrySHA holds the resolved revision (sha) of the dry source as of the most recent reconciliation\"\n    },\n    \"hydratedSHA\": {\n      \"type\": \"string\",\n      \"title\": \"HydratedSHA holds the resolved revision (sha) of the hydrated source as of the most recent reconciliation\"\n    },\n    \"sourceHydrator\": {\n      \"$ref\": \"#/definitions/v1alpha1SourceHydrator\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-successful-hydrate-operation-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SuccessfulHydrateOperation
---
