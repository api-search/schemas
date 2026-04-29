---
description: Details about the EKS cluster involved in a Kubernetes finding.
layout: schema
name: EksClusterDetails
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: CreatedAt
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-eks-cluster-details-schema.json
slug: guardduty-eks-cluster-details
source_filename: guardduty-eks-cluster-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-eks-cluster-details-schema.json\",\n  \"title\": \"EksClusterDetails\",\n  \"description\": \"Details about the EKS cluster involved in a Kubernetes finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"EKS cluster name.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"EKS cluster ARN.\"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcId\"\n          },\n          \"description\": \"The VPC ID to which the EKS cluster is attached.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The EKS cluster status.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The EKS cluster tags.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n        \
  \  },\n          \"description\": \"The timestamp when the EKS cluster was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-eks-cluster-details-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: EksClusterDetails
---
