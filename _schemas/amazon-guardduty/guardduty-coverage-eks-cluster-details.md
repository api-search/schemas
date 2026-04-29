---
description: Information about the EKS cluster that has a coverage status.
layout: schema
name: CoverageEksClusterDetails
properties_list:
- description: ''
  name: ClusterName
  type: object
- description: ''
  name: CoveredNodes
  type: object
- description: ''
  name: CompatibleNodes
  type: object
- description: ''
  name: AddonDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-eks-cluster-details-schema.json
slug: guardduty-coverage-eks-cluster-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-eks-cluster-details-schema.json\",\n  \"title\": \"CoverageEksClusterDetails\",\n  \"description\": \"Information about the EKS cluster that has a coverage status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterName\"\n          },\n          \"description\": \"Name of the EKS cluster.\"\n        }\n      ]\n    },\n    \"CoveredNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"coveredNodes\"\n          },\n          \"description\": \"Represents the nodes within the EKS cluster that have\
  \ a <code>HEALTHY</code> coverage status.\"\n        }\n      ]\n    },\n    \"CompatibleNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"compatibleNodes\"\n          },\n          \"description\": \"Represents all the nodes within the EKS cluster in your account.\"\n        }\n      ]\n    },\n    \"AddonDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddonDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"addonDetails\"\n          },\n          \"description\": \"Information about the installed EKS add-on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-eks-cluster-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageEksClusterDetails
---
