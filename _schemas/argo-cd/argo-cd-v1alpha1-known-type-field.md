---
description: KnownTypeField contains a mapping between a Custom Resource Definition (CRD) field and a well-known Kubernetes type. This mapping is primarily used for unit conversions in resources where the type is not explicitly defined (e.g., converting "0.1" to "100m" for CPU requests).
layout: schema
name: v1alpha1KnownTypeField
properties_list:
- description: ''
  name: field
  type: string
- description: Type specifies the expected Kubernetes type for the field, such as "cpu" or "memory". This helps in converting values between different formats (e.g., "0.1" to "100m" for CPU).
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-known-type-field-schema.json
slug: argo-cd-v1alpha1-known-type-field
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1KnownTypeField
---
