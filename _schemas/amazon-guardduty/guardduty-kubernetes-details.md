---
description: Details about Kubernetes resources such as a Kubernetes user or workload resource involved in a Kubernetes finding.
layout: schema
name: KubernetesDetails
properties_list:
- description: ''
  name: KubernetesUserDetails
  type: object
- description: ''
  name: KubernetesWorkloadDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-details-schema.json
slug: guardduty-kubernetes-details
source_filename: guardduty-kubernetes-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-details-schema.json\",\n  \"title\": \"KubernetesDetails\",\n  \"description\": \"Details about Kubernetes resources such as a Kubernetes user or workload resource involved in a Kubernetes finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KubernetesUserDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesUserDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetesUserDetails\"\n          },\n          \"description\": \"Details about the Kubernetes user involved in a Kubernetes finding.\"\n        }\n      ]\n    },\n    \"KubernetesWorkloadDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesWorkloadDetails\"\n        },\n        {\n         \
  \ \"xml\": {\n            \"name\": \"kubernetesWorkloadDetails\"\n          },\n          \"description\": \"Details about the Kubernetes workload involved in a Kubernetes finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesDetails
---
