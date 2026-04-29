---
description: Details about the Kubernetes user involved in a Kubernetes finding.
layout: schema
name: KubernetesUserDetails
properties_list:
- description: ''
  name: Username
  type: object
- description: ''
  name: Uid
  type: object
- description: ''
  name: Groups
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-user-details-schema.json
slug: guardduty-kubernetes-user-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-user-details-schema.json\",\n  \"title\": \"KubernetesUserDetails\",\n  \"description\": \"Details about the Kubernetes user involved in a Kubernetes finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"The username of the user who called the Kubernetes API.\"\n        }\n      ]\n    },\n    \"Uid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uid\"\n          },\n          \"description\": \"The user ID of the user who called the Kubernetes\
  \ API.\"\n        }\n      ]\n    },\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Groups\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"groups\"\n          },\n          \"description\": \"The groups that include the user who called the Kubernetes API.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-user-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesUserDetails
---
