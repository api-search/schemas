---
description: v1alpha1ApplicationDestination schema from Argo CD API
layout: schema
name: v1alpha1ApplicationDestination
properties_list:
- description: Name is an alternate way of specifying the target cluster by its symbolic name. This must be set if Server is not set.
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: Server specifies the URL of the target cluster's Kubernetes control plane API. This must be set if Name is not set.
  name: server
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-destination-schema.json
slug: argo-cd-v1alpha1-application-destination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-destination-schema.json\",\n  \"title\": \"v1alpha1ApplicationDestination\",\n  \"description\": \"v1alpha1ApplicationDestination schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name is an alternate way of specifying the target cluster by its symbolic name. This must be set if Server is not set.\",\n      \"type\": \"string\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"title\": \"Namespace specifies the target namespace for the application's resources.\\nThe namespace will only be set for namespace-scoped resources that have not set a value for .metadata.namespace\"\n    },\n    \"server\": {\n      \"description\": \"Server specifies the URL of the target cluster's Kubernetes control plane\
  \ API. This must be set if Name is not set.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-destination-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationDestination
---
