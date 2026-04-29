---
description: Details about the Kubernetes workload involved in a Kubernetes finding.
layout: schema
name: KubernetesWorkloadDetails
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Uid
  type: object
- description: ''
  name: Namespace
  type: object
- description: ''
  name: HostNetwork
  type: object
- description: ''
  name: Containers
  type: object
- description: ''
  name: Volumes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-workload-details-schema.json
slug: guardduty-kubernetes-workload-details
source_filename: guardduty-kubernetes-workload-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-workload-details-schema.json\",\n  \"title\": \"KubernetesWorkloadDetails\",\n  \"description\": \"Details about the Kubernetes workload involved in a Kubernetes finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Kubernetes workload name.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"Kubernetes workload type (e.g. Pod, Deployment, etc.).\"\n        }\n \
  \     ]\n    },\n    \"Uid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uid\"\n          },\n          \"description\": \"Kubernetes workload ID.\"\n        }\n      ]\n    },\n    \"Namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"namespace\"\n          },\n          \"description\": \"Kubernetes namespace that the workload is part of.\"\n        }\n      ]\n    },\n    \"HostNetwork\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostNetwork\"\n          },\n          \"description\": \"Whether the hostNetwork flag is enabled for the pods included in the workload.\"\n        }\n      ]\n    },\n    \"Containers\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/Containers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containers\"\n          },\n          \"description\": \"Containers running as part of the Kubernetes workload.\"\n        }\n      ]\n    },\n    \"Volumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Volumes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumes\"\n          },\n          \"description\": \"Volumes used by the Kubernetes workload.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-workload-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesWorkloadDetails
---
