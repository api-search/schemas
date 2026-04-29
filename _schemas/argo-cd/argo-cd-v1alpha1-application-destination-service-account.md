---
description: ApplicationDestinationServiceAccount holds information about the service account to be impersonated for the application sync operation.
layout: schema
name: v1alpha1ApplicationDestinationServiceAccount
properties_list:
- description: ''
  name: defaultServiceAccount
  type: string
- description: Namespace specifies the target namespace for the application's resources.
  name: namespace
  type: string
- description: Server specifies the URL of the target cluster's Kubernetes control plane API.
  name: server
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-destination-service-account-schema.json
slug: argo-cd-v1alpha1-application-destination-service-account
source_filename: argo-cd-v1alpha1-application-destination-service-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-destination-service-account-schema.json\",\n  \"title\": \"v1alpha1ApplicationDestinationServiceAccount\",\n  \"description\": \"ApplicationDestinationServiceAccount holds information about the service account to be impersonated for the application sync operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultServiceAccount\": {\n      \"type\": \"string\",\n      \"title\": \"DefaultServiceAccount to be used for impersonation during the sync operation\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace specifies the target namespace for the application's resources.\",\n      \"type\": \"string\"\n    },\n    \"server\": {\n      \"description\": \"Server specifies the URL of the target cluster's Kubernetes control plane API.\",\n      \"type\": \"\
  string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-destination-service-account-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationDestinationServiceAccount
---
