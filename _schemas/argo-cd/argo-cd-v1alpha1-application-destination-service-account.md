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
