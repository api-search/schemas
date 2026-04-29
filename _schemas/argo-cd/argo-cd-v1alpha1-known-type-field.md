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
source_filename: argo-cd-v1alpha1-known-type-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-known-type-field-schema.json\",\n  \"title\": \"v1alpha1KnownTypeField\",\n  \"description\": \"KnownTypeField contains a mapping between a Custom Resource Definition (CRD) field\\nand a well-known Kubernetes type. This mapping is primarily used for unit conversions\\nin resources where the type is not explicitly defined (e.g., converting \\\"0.1\\\" to \\\"100m\\\" for CPU requests).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\",\n      \"title\": \"Field represents the JSON path to the specific field in the CRD that requires type conversion.\\nExample: \\\"spec.resources.requests.cpu\\\"\"\n    },\n    \"type\": {\n      \"description\": \"Type specifies the expected Kubernetes type for the field, such as \\\"cpu\\\" or \\\"memory\\\".\\nThis\
  \ helps in converting values between different formats (e.g., \\\"0.1\\\" to \\\"100m\\\" for CPU).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-known-type-field-schema.json
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
